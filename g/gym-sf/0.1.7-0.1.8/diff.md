# Comparing `tmp/gym-sf-0.1.7.tar.gz` & `tmp/gym-sf-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-sf-0.1.7.tar", last modified: Fri Apr 28 15:30:15 2023, max compression
+gzip compressed data, was "gym-sf-0.1.8.tar", last modified: Fri Apr 28 16:02:39 2023, max compression
```

## Comparing `gym-sf-0.1.7.tar` & `gym-sf-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.098000 gym-sf-0.1.7/
--rw-rw-rw-   0        0        0     1091 2022-09-08 13:48:37.000000 gym-sf-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0      301 2023-04-28 15:30:15.090000 gym-sf-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2728 2022-10-21 14:03:57.000000 gym-sf-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 15:30:14.874000 gym-sf-0.1.7/gym_sf/
--rw-rw-rw-   0        0        0       27 2022-10-21 13:28:35.000000 gym-sf-0.1.7/gym_sf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.025000 gym-sf-0.1.7/gym_sf/four_room/
--rw-rw-rw-   0        0        0      367 2023-01-16 12:34:38.000000 gym-sf-0.1.7/gym_sf/four_room/__init__.py
--rw-rw-rw-   0        0        0      732 2022-11-10 14:43:13.000000 gym-sf-0.1.7/gym_sf/four_room/example.py
--rw-rw-rw-   0        0        0     9562 2023-03-14 23:42:43.000000 gym-sf-0.1.7/gym_sf/four_room/four_room.py
--rw-rw-rw-   0        0        0     5563 2023-04-28 11:59:31.000000 gym-sf-0.1.7/gym_sf/four_room/four_room_goalEnv.py
--rw-rw-rw-   0        0        0     7164 2023-03-14 23:43:00.000000 gym-sf-0.1.7/gym_sf/four_room/render.py
--rw-rw-rw-   0        0        0      805 2022-11-10 16:44:07.000000 gym-sf-0.1.7/gym_sf/four_room/trial.py
--rw-rw-rw-   0        0        0      796 2022-12-21 14:59:53.000000 gym-sf-0.1.7/gym_sf/four_room/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:30:15.078000 gym-sf-0.1.7/gym_sf/four_room_multiagent/
--rw-rw-rw-   0        0        0      254 2023-01-16 12:30:08.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-04-28 14:58:53.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/example_mult.py
--rw-rw-rw-   0        0        0    10008 2023-04-28 14:26:10.000000 gym-sf-0.1.7/gym_sf/four_room_multiagent/four_room_multiagent.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:30:14.929000 gym-sf-0.1.7/gym_sf.egg-info/
--rw-rw-rw-   0        0        0      301 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 15:30:14.000000 gym-sf-0.1.7/gym_sf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 15:30:15.096000 gym-sf-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-04-28 14:18:28.000000 gym-sf-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:02:39.434000 gym-sf-0.1.8/
+-rw-rw-rw-   0        0        0     1091 2022-09-08 13:48:37.000000 gym-sf-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      301 2023-04-28 16:02:39.425000 gym-sf-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2728 2022-10-21 14:03:57.000000 gym-sf-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 16:02:39.238000 gym-sf-0.1.8/gym_sf/
+-rw-rw-rw-   0        0        0       27 2022-10-21 13:28:35.000000 gym-sf-0.1.8/gym_sf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:02:39.378000 gym-sf-0.1.8/gym_sf/four_room/
+-rw-rw-rw-   0        0        0      367 2023-01-16 12:34:38.000000 gym-sf-0.1.8/gym_sf/four_room/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-11-10 14:43:13.000000 gym-sf-0.1.8/gym_sf/four_room/example.py
+-rw-rw-rw-   0        0        0     9562 2023-03-14 23:42:43.000000 gym-sf-0.1.8/gym_sf/four_room/four_room.py
+-rw-rw-rw-   0        0        0     5563 2023-04-28 11:59:31.000000 gym-sf-0.1.8/gym_sf/four_room/four_room_goalEnv.py
+-rw-rw-rw-   0        0        0     7164 2023-03-14 23:43:00.000000 gym-sf-0.1.8/gym_sf/four_room/render.py
+-rw-rw-rw-   0        0        0      805 2022-11-10 16:44:07.000000 gym-sf-0.1.8/gym_sf/four_room/trial.py
+-rw-rw-rw-   0        0        0      796 2022-12-21 14:59:53.000000 gym-sf-0.1.8/gym_sf/four_room/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:02:39.416000 gym-sf-0.1.8/gym_sf/four_room_multiagent/
+-rw-rw-rw-   0        0        0      254 2023-01-16 12:30:08.000000 gym-sf-0.1.8/gym_sf/four_room_multiagent/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-04-28 14:58:53.000000 gym-sf-0.1.8/gym_sf/four_room_multiagent/example_mult.py
+-rw-rw-rw-   0        0        0     8943 2023-04-28 16:00:16.000000 gym-sf-0.1.8/gym_sf/four_room_multiagent/four_room_multiagent.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:02:39.293000 gym-sf-0.1.8/gym_sf.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-04-28 16:02:39.000000 gym-sf-0.1.8/gym_sf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-28 16:02:39.000000 gym-sf-0.1.8/gym_sf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:02:39.000000 gym-sf-0.1.8/gym_sf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-28 16:02:39.000000 gym-sf-0.1.8/gym_sf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 16:02:39.000000 gym-sf-0.1.8/gym_sf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 16:02:39.432000 gym-sf-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-04-28 16:02:24.000000 gym-sf-0.1.8/setup.py
```

### Comparing `gym-sf-0.1.7/LICENSE.txt` & `gym-sf-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/README.md` & `gym-sf-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/example.py` & `gym-sf-0.1.8/gym_sf/four_room/example.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/four_room.py` & `gym-sf-0.1.8/gym_sf/four_room/four_room.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/four_room_goalEnv.py` & `gym-sf-0.1.8/gym_sf/four_room/four_room_goalEnv.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/render.py` & `gym-sf-0.1.8/gym_sf/four_room/render.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/trial.py` & `gym-sf-0.1.8/gym_sf/four_room/trial.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room/utilities.py` & `gym-sf-0.1.8/gym_sf/four_room/utilities.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room_multiagent/example_mult.py` & `gym-sf-0.1.8/gym_sf/four_room_multiagent/example_mult.py`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/gym_sf/four_room_multiagent/four_room_multiagent.py` & `gym-sf-0.1.8/gym_sf/four_room_multiagent/four_room_multiagent.py`

 * *Files 12% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         return self.state_to_array(self.state), info
 
 
     def step(self, actions):
         reward = 0.
         self.step_count += 1
         collected = self.state[1]
-        actions = self.action_dict[str(actions)]
+        actions = self.action_dict[actions]
         for i in range(self.max_num_agents):
             if self.max_num_agents == 1:
                 (row, col) = self.state[0]
                 action = actions[0]
             else:
                 (row, col) = self.state[0][i]
                 action = actions[i]
@@ -223,40 +223,7 @@
         if self.render_mode == 'human':
             self.my_render.update(self.state[0], mode=self.render_mode)
         elif self.render_mode == 'rgb_array':  # rgb_array or single_rgb_array
             return self.my_render.update(self.state[0], mode=self.render_mode)
         elif self.render_mode == 'rgb_array_list':
             self.frames.append(self.my_render.update(self.state[0], mode=self.render_mode))
 
-
-if __name__ == '__main__':
-
-    import os
-
-    # render_mode = "rgb_array_list" # "rgb_array" "rgb_array_list"
-    render_mode = 'human'
-    video_path = os.getcwd()
-    # num_agents = 2
-
-    num_agents = 2
-
-    env = gym.make("four-room-multiagent-v0", render_mode=render_mode, max_episode_steps=5000,
-                video=True, video_path=video_path, max_num_agents=num_agents, given_initial_position=False)
-    # env = gym.make("four-room-v0", render_mode='human', new_step_api=True, max_episode_steps=5000)
-    terminated = False
-    truncated = False
-    env.reset()
-
-    for _ in range(500):
-        action = env.action_space.sample()
-        for agent in range(num_agents):
-            if np.random.random() < 0.20:
-                if np.random.random() < 0.50:
-                    action = 2
-                else:
-                    action = 1
-        next_state, reward, terminated, truncated, _ = env.step(action)
-
-        if terminated or truncated:
-            env.render()
-            env.reset()
-    env.close()
```

### Comparing `gym-sf-0.1.7/gym_sf.egg-info/SOURCES.txt` & `gym-sf-0.1.8/gym_sf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym-sf-0.1.7/setup.py` & `gym-sf-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 packages = [package for package in find_packages() if package.startswith("gym_sf")]
 
 setup(name='gym-sf',
-      version='0.1.7',
+      version='0.1.8',
       description='Environments adapted to the use of successor features',
       author="Rafael F Cunha",
       author_email="rafaelcunha2013@gmail.com",
       url="https://github.com/rafaelcunha2013/gym-sf",
       license='MIT',
       packages=packages,
       python_requires=">=3.8",
```

