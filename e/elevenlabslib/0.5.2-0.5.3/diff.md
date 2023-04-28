# Comparing `tmp/elevenlabslib-0.5.2.tar.gz` & `tmp/elevenlabslib-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.5.2.tar", last modified: Wed Apr 26 11:48:17 2023, max compression
+gzip compressed data, was "elevenlabslib-0.5.3.tar", last modified: Fri Apr 28 09:19:30 2023, max compression
```

## Comparing `elevenlabslib-0.5.2.tar` & `elevenlabslib-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.516280 elevenlabslib-0.5.2/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     2706 2023-04-26 11:48:17.515279 elevenlabslib-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.501279 elevenlabslib-0.5.2/elevenlabslib/
--rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    13370 2023-04-26 11:22:54.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    31137 2023-04-25 19:23:19.000000 elevenlabslib-0.5.2/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.5.2/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5524 2023-04-26 11:42:12.000000 elevenlabslib-0.5.2/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-26 11:48:17.515279 elevenlabslib-0.5.2/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2706 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 11:48:17.000000 elevenlabslib-0.5.2/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      856 2023-04-26 11:46:48.000000 elevenlabslib-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 11:48:17.516280 elevenlabslib-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.768159 elevenlabslib-0.5.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     2706 2023-04-28 09:19:30.767163 elevenlabslib-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.752162 elevenlabslib-0.5.3/elevenlabslib/
+-rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    13846 2023-04-28 09:10:06.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    31783 2023-04-28 09:17:07.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.5.3/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5524 2023-04-26 11:42:12.000000 elevenlabslib-0.5.3/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.766159 elevenlabslib-0.5.3/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2706 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      856 2023-04-28 09:17:16.000000 elevenlabslib-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:19:30.768159 elevenlabslib-0.5.3/setup.cfg
```

### Comparing `elevenlabslib-0.5.2/LICENSE` & `elevenlabslib-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.2/PKG-INFO` & `elevenlabslib-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.2
+Version: 0.5.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.5.2/README.md` & `elevenlabslib-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,29 @@
     def headers(self) -> dict:
         """
         Returns:
             dict: The headers used for API requests.
         """
         return self._headers
 
+    def get_available_models(self) -> list[dict]:
+        """
+        This function returns all the available models for this account.
+
+        Note:
+            You can use the model_id from a model's info for calls to the text to speech endpoint.
+
+        Returns:
+            list[dict]: All the available models for this account.
+        """
+        response = _api_get("/models", self._headers)
+        userData = response.json()
+        return userData
+
+
     def get_user_data(self) -> dict:
         """
         Returns:
              dict: All the information returned by the /v1/user endpoint.
         """
         response = _api_get("/user/subscription", self._headers)
         userData = response.json()
```

### Comparing `elevenlabslib-0.5.2/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsVoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,63 +140,63 @@
             if similarity_boost is None: stability = oldSettings["similarity_boost"]
 
         if not(0 <= stability <= 1 and 0 <= similarity_boost <= 1):
             raise ValueError("Please provide a value between 0 and 1.")
         payload = {"stability": stability, "similarity_boost": similarity_boost}
         _api_json("/voices/" + self._voiceID + "/settings/edit", self._linkedUser.headers, jsonData=payload)
 
-    def _generate_payload(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None) -> dict:
+    def _generate_payload(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None, model_id:str="eleven_monolingual_v1") -> dict:
         """
         Generates the payload for the text-to-speech API call.
 
         Args:
             prompt (str): The prompt to generate speech for.
             stability (Optional[float]): A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost (Optional[float]): A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
-
+            model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
         Returns:
             dict: A dictionary representing the payload for the API call.
         """
-        payload = {"text": prompt}
+        payload = {"text": prompt, "model_id": model_id}
         if stability is not None or similarity_boost is not None:
             currentSettings = self.get_settings()
             if stability is None: stability = currentSettings["stability"]
             if similarity_boost is None: similarity_boost = currentSettings["similarity_boost"]
             if not (0 <= stability <= 1 and 0 <= similarity_boost <= 1):
                 raise ValueError("Please provide a value between 0 and 1.")
             payload["voice_settings"] = dict()
             payload["voice_settings"]["stability"] = stability
             payload["voice_settings"]["similarity_boost"] = similarity_boost
         return payload
 
-    def generate_audio_bytes(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None) -> bytes:
+    def generate_audio_bytes(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None, model_id:str="eleven_monolingual_v1") -> bytes:
         """
         Generates speech for the given prompt and returns the audio data as bytes of an mp3 file.
 
         Tip:
             If you would like to save the audio to disk or otherwise, you can use helpers.save_audio_bytes().
 
         Args:
         	prompt: The prompt to generate speech for.
         	stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
         	similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
-
+        	model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
         Returns:
         	The bytes of the audio file.
 
         """
-        payload = self._generate_payload(prompt, stability, similarity_boost)
+        payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
 
         return response.content
 
     def generate_and_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
-                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None):
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1"):
         """
         Generate audio bytes from the given prompt and play them using sounddevice.
 
         Tip:
             This function downloads the entire file before playing it back, and even if playInBackground is set, it will halt execution until the file is downloaded.
             If you need faster response times and background downloading and playback, use generate_and_stream_audio.
 
@@ -204,25 +204,26 @@
         	prompt (str): The text prompt to generate audio from.
         	playInBackground (bool): Whether to play audio in the background or wait for it to finish playing.
         	portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
         	stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
         	similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
         	onPlaybackStart: Function to call once the playback begins
         	onPlaybackEnd: Function to call once the playback ends
+        	model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
 
         Returns:
             The audio bytes.
         """
-        audioData = self.generate_audio_bytes(prompt, stability, similarity_boost)
+        audioData = self.generate_audio_bytes(prompt, stability, similarity_boost, model_id)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
         return audioData
 
     def generate_and_stream_audio(self, prompt:str, portaudioDeviceID:Optional[int] = None,
                                   stability:Optional[float]=None, similarity_boost:Optional[float]=None, streamInBackground=False,
-                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None):
+                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1"):
         """
 
         Note:
             No longer suffers from the skipping issues it had in the past.
 
         Generate audio bytes from the given prompt and stream them using sounddevice.
 
@@ -232,17 +233,18 @@
             streamInBackground (bool): Whether or not to play the audio (and let the download complete) in a separate thread.
             prompt (str): The text prompt to generate audio from.
             portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
+            model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
 
         """
-        payload = self._generate_payload(prompt, stability, similarity_boost)
+        payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         path = "/text-to-speech/" + self._voiceID + "/stream"
 
         streamedResponse = requests.post(api_endpoint + path, headers=self._linkedUser.headers, json=payload, stream=True)
 
         streamer = _AudioChunkStreamer(portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
         if streamInBackground:
```

### Comparing `elevenlabslib-0.5.2/elevenlabslib/helpers.py` & `elevenlabslib-0.5.3/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.2/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.5.3/elevenlabslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.2
+Version: 0.5.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.5.2/pyproject.toml` & `elevenlabslib-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

