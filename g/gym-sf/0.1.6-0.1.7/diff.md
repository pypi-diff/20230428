# Comparing `tmp/gym-sf-0.1.6.tar.gz` & `tmp/gym-sf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-sf-0.1.6.tar", last modified: Tue Mar 14 23:46:36 2023, max compression
+gzip compressed data, was "gym-sf-0.1.7.tar", last modified: Fri Apr 28 15:30:15 2023, max compression
```

## Comparing `gym-sf-0.1.6.tar` & `gym-sf-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rafaelfernandescunha   (501) staff       (20)        0 2023-03-14 23:46:36.405457 gym-sf-0.1.6/
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     1091 2022-09-08 13:48:37.000000 gym-sf-0.1.6/LICENSE.txt
--rw-r--r--   0 rafaelfernandescunha   (501) staff       (20)      319 2023-03-14 23:46:36.403692 gym-sf-0.1.6/PKG-INFO
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     2728 2022-10-21 14:03:57.000000 gym-sf-0.1.6/README.md
-drwxr-xr-x   0 rafaelfernandescunha   (501) staff       (20)        0 2023-03-14 23:46:36.372637 gym-sf-0.1.6/gym_sf/
--rw-------   0 rafaelfernandescunha   (501) staff       (20)       27 2022-10-21 13:28:35.000000 gym-sf-0.1.6/gym_sf/__init__.py
-drwxr-xr-x   0 rafaelfernandescunha   (501) staff       (20)        0 2023-03-14 23:46:36.391992 gym-sf-0.1.6/gym_sf/four_room/
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      367 2023-01-16 12:34:38.000000 gym-sf-0.1.6/gym_sf/four_room/__init__.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      732 2022-11-10 14:43:13.000000 gym-sf-0.1.6/gym_sf/four_room/example.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     9562 2023-03-14 23:42:37.000000 gym-sf-0.1.6/gym_sf/four_room/four_room.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     5563 2023-02-06 13:49:53.000000 gym-sf-0.1.6/gym_sf/four_room/four_room_goalEnv.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     7164 2023-03-14 23:42:54.000000 gym-sf-0.1.6/gym_sf/four_room/render.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      805 2022-11-10 16:44:07.000000 gym-sf-0.1.6/gym_sf/four_room/trial.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      796 2022-12-21 14:59:53.000000 gym-sf-0.1.6/gym_sf/four_room/utilities.py
-drwxr-xr-x   0 rafaelfernandescunha   (501) staff       (20)        0 2023-03-14 23:46:36.401981 gym-sf-0.1.6/gym_sf/four_room_multiagent/
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      254 2023-01-16 12:30:08.000000 gym-sf-0.1.6/gym_sf/four_room_multiagent/__init__.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      926 2023-01-16 18:27:38.000000 gym-sf-0.1.6/gym_sf/four_room_multiagent/example_mult.py
--rw-------   0 rafaelfernandescunha   (501) staff       (20)     8205 2023-03-14 23:42:13.000000 gym-sf-0.1.6/gym_sf/four_room_multiagent/four_room_multiagent.py
-drwxr-xr-x   0 rafaelfernandescunha   (501) staff       (20)        0 2023-03-14 23:46:36.376823 gym-sf-0.1.6/gym_sf.egg-info/
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      319 2023-03-14 23:46:28.000000 gym-sf-0.1.6/gym_sf.egg-info/PKG-INFO
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      542 2023-03-14 23:46:36.000000 gym-sf-0.1.6/gym_sf.egg-info/SOURCES.txt
--rw-------   0 rafaelfernandescunha   (501) staff       (20)        1 2023-03-14 23:46:30.000000 gym-sf-0.1.6/gym_sf.egg-info/dependency_links.txt
--rw-------   0 rafaelfernandescunha   (501) staff       (20)       48 2023-03-14 23:46:32.000000 gym-sf-0.1.6/gym_sf.egg-info/requires.txt
--rw-------   0 rafaelfernandescunha   (501) staff       (20)        7 2023-03-14 23:46:34.000000 gym-sf-0.1.6/gym_sf.egg-info/top_level.txt
--rw-r--r--   0 rafaelfernandescunha   (501) staff       (20)       38 2023-03-14 23:46:36.405751 gym-sf-0.1.6/setup.cfg
--rw-------   0 rafaelfernandescunha   (501) staff       (20)      809 2023-03-14 23:46:20.000000 gym-sf-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.098000 gym-sf-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2022-09-08 13:48:37.000000 gym-sf-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      301 2023-04-28 15:30:15.090000 gym-sf-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2728 2022-10-21 14:03:57.000000 gym-sf-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:30:14.874000 gym-sf-0.1.7/gym_sf/
+-rw-rw-rw-   0        0        0       27 2022-10-21 13:28:35.000000 gym-sf-0.1.7/gym_sf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.025000 gym-sf-0.1.7/gym_sf/four_room/
+-rw-rw-rw-   0        0        0      367 2023-01-16 12:34:38.000000 gym-sf-0.1.7/gym_sf/four_room/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-11-10 14:43:13.000000 gym-sf-0.1.7/gym_sf/four_room/example.py
+-rw-rw-rw-   0        0        0     9562 2023-03-14 23:42:43.000000 gym-sf-0.1.7/gym_sf/four_room/four_room.py
+-rw-rw-rw-   0        0        0     5563 2023-04-28 11:59:31.000000 gym-sf-0.1.7/gym_sf/four_room/four_room_goalEnv.py
+-rw-rw-rw-   0        0        0     7164 2023-03-14 23:43:00.000000 gym-sf-0.1.7/gym_sf/four_room/render.py
+-rw-rw-rw-   0        0        0      805 2022-11-10 16:44:07.000000 gym-sf-0.1.7/gym_sf/four_room/trial.py
+-rw-rw-rw-   0        0        0      796 2022-12-21 14:59:53.000000 gym-sf-0.1.7/gym_sf/four_room/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.078000 gym-sf-0.1.7/gym_sf/four_room_multiagent/
+-rw-rw-rw-   0        0        0      254 2023-01-16 12:30:08.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-04-28 14:58:53.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/example_mult.py
+-rw-rw-rw-   0        0        0    10008 2023-04-28 14:26:10.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/four_room_multiagent.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:30:14.929000 gym-sf-0.1.7/gym_sf.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:30:15.096000 gym-sf-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-04-28 14:18:28.000000 gym-sf-0.1.7/setup.py
```

### Comparing `gym-sf-0.1.6/LICENSE.txt` & `gym-sf-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/README.md` & `gym-sf-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/example.py` & `gym-sf-0.1.7/gym_sf/four_room/example.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/four_room.py` & `gym-sf-0.1.7/gym_sf/four_room/four_room.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/four_room_goalEnv.py` & `gym-sf-0.1.7/gym_sf/four_room/four_room_goalEnv.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/render.py` & `gym-sf-0.1.7/gym_sf/four_room/render.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/trial.py` & `gym-sf-0.1.7/gym_sf/four_room/trial.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room/utilities.py` & `gym-sf-0.1.7/gym_sf/four_room/utilities.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/gym_sf/four_room_multiagent/four_room_multiagent.py` & `gym-sf-0.1.7/gym_sf/four_room_multiagent/four_room_multiagent.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,70 +21,87 @@
     ['_', ' ', ' ', ' ', ' ', ' ', 'X', '2', ' ', ' ', ' ', ' ', '3'],
     [' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', ' ', ' ', ' ', ' ', ' '],
     [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '],
     [' ', ' ', ' ', ' ', ' ', ' ', '2', ' ', ' ', ' ', ' ', ' ', ' '],
     [' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', ' ', ' ', ' ', ' ', ' '],
     [' ', ' ', ' ', ' ', ' ', '_', 'X', '3', ' ', ' ', ' ', ' ', '1']])
 REWARDS = dict(zip(['1', '2', '3'], list([1.0, 0.5, -1.0])))
-action_conversion = [('0', [0, 0]),
-                     ('1', [1, 0]),
-                     ('2', [2, 0]),
-                     ('3', [3, 0]),
-                     ('4', [0, 1]),
-                     ('5', [1, 1]),
-                     ('6', [2, 1]),
-                     ('7', [3, 1]),
-                     ('8', [0, 2]),
-                     ('9', [1, 2]),
-                     ('10', [2, 2]),
-                     ('11', [3, 2]),
-                     ('12', [0, 3]),
-                     ('13', [1, 3]),
-                     ('14', [2, 3]),
-                     ('15', [3, 3])]
-action_dict = dict(action_conversion)
-
-# action_dict = dict()
-# for i in range(16):
-#     action_dict[i] = [i % 4, i // 4]
+# action_conversion = [('0', [0, 0]),
+#                      ('1', [1, 0]),
+#                      ('2', [2, 0]),
+#                      ('3', [3, 0]),
+#                      ('4', [0, 1]),
+#                      ('5', [1, 1]),
+#                      ('6', [2, 1]),
+#                      ('7', [3, 1]),
+#                      ('8', [0, 2]),
+#                      ('9', [1, 2]),
+#                      ('10', [2, 2]),
+#                      ('11', [3, 2]),
+#                      ('12', [0, 3]),
+#                      ('13', [1, 3]),
+#                      ('14', [2, 3]),
+#                      ('15', [3, 3])]
+# action_dict = dict(action_conversion)
+
+action_dict = dict()
+for i in range(16):
+    action_dict[i] = [i % 4, i // 4]
 
 
 class FourRoomMultiagent(FourRoom):
     """
     Four room environment suitable for two agents
     """
     def __init__(self, maze=MAZE, shape_rewards=REWARDS,
                  render_mode='rgb_array', random_initial_position=True, video=False,
-                 video_path='root', max_num_agents=2):
+                 video_path='root', max_num_agents=2, initial_position=[(12,0)], given_initial_position=False):
         super().__init__(maze=maze, shape_rewards=shape_rewards,
                  render_mode=render_mode, random_initial_position=random_initial_position, video=video,
                  video_path=video_path)
         self.max_num_agents = max_num_agents
         self.action_space = spaces.Discrete(4 ** max_num_agents)
         self.observation_space = spaces.Box(low=np.zeros(2*max_num_agents + len(self.shape_ids)),
                                             high=len(self.maze) * np.ones(2*max_num_agents + len(self.shape_ids)),
                                             dtype=np.int32)
         self.action_dict = action_dict
+        self.given_initial_position = given_initial_position
+        self.init_position = initial_position
 
-    def random_position(self):
+    def erase_maze_position(self):
         for c in range(self.width):
             for r in range(self.height):
                 if self.env_maze[r, c] == '_':
-                    self.env_maze[r, c] = ' '
+                    self.env_maze[r, c] = ' '      
+
+    
+    def random_position(self):
+        self.erase_maze_position()
+        # for c in range(self.width):
+        #     for r in range(self.height):
+        #         if self.env_maze[r, c] == '_':
+        #             self.env_maze[r, c] = ' '
         self.initial = []
         n_r, n_c = np.shape(self.maze)
         for _ in range(self.max_num_agents):
             initial_position = False
             while not initial_position:
                 r, c = (np.random.randint(0, n_r), np.random.randint(0, n_c))
                 if self.maze[r, c] == ' ':
                     self.initial.append((r, c))
                     self.env_maze[r, c] = '_'
                     initial_position = True
 
+    def given_position(self):
+        self.erase_maze_position()
+        self.initial = self.init_position 
+        for r, c in self.init_position:      
+            self.env_maze[r, c] = '_'
+
+
     @staticmethod
     def state_to_array(state):
         if isinstance(state[0][0], tuple):
             s_agent = [element for tupl in state[0] for element in tupl]
             s_objects = list(state[1])
             s = s_agent + s_objects
         else:
@@ -93,14 +110,16 @@
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed)
         self.step_count = 0
         self.truncated = False
         self.terminated = False
         self.env_maze = copy.deepcopy(self.maze)
+        if self.given_initial_position:
+            self.given_position()
         if self.random_initial_position:
             self.random_position()
         if self.max_num_agents == 1:
             self.state = (random.choice(self.initial), tuple(0 for _ in range(len(self.shape_ids))))
         else:
             self.state = (self.initial, tuple(0 for _ in range(len(self.shape_ids))))
         self.my_render = Render(maze=self.env_maze, render_mode=self.render_mode)
@@ -202,8 +221,42 @@
 
     def _render_frame(self):
         if self.render_mode == 'human':
             self.my_render.update(self.state[0], mode=self.render_mode)
         elif self.render_mode == 'rgb_array':  # rgb_array or single_rgb_array
             return self.my_render.update(self.state[0], mode=self.render_mode)
         elif self.render_mode == 'rgb_array_list':
-            self.frames.append(self.my_render.update(self.state[0], mode=self.render_mode))
+            self.frames.append(self.my_render.update(self.state[0], mode=self.render_mode))
+
+
+if __name__ == '__main__':
+
+    import os
+
+    # render_mode = "rgb_array_list" # "rgb_array" "rgb_array_list"
+    render_mode = 'human'
+    video_path = os.getcwd()
+    # num_agents = 2
+
+    num_agents = 2
+
+    env = gym.make("four-room-multiagent-v0", render_mode=render_mode, max_episode_steps=5000,
+                video=True, video_path=video_path, max_num_agents=num_agents, given_initial_position=False)
+    # env = gym.make("four-room-v0", render_mode='human', new_step_api=True, max_episode_steps=5000)
+    terminated = False
+    truncated = False
+    env.reset()
+
+    for _ in range(500):
+        action = env.action_space.sample()
+        for agent in range(num_agents):
+            if np.random.random() < 0.20:
+                if np.random.random() < 0.50:
+                    action = 2
+                else:
+                    action = 1
+        next_state, reward, terminated, truncated, _ = env.step(action)
+
+        if terminated or truncated:
+            env.render()
+            env.reset()
+    env.close()
```

### Comparing `gym-sf-0.1.6/gym_sf.egg-info/SOURCES.txt` & `gym-sf-0.1.7/gym_sf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.6/setup.py` & `gym-sf-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 packages = [package for package in find_packages() if package.startswith("gym_sf")]
 
 setup(name='gym-sf',
-      version='0.1.6',
+      version='0.1.7',
       description='Environments adapted to the use of successor features',
       author="Rafael F Cunha",
       author_email="rafaelcunha2013@gmail.com",
       url="https://github.com/rafaelcunha2013/gym-sf",
       license='MIT',
       packages=packages,
       python_requires=">=3.8",
```

