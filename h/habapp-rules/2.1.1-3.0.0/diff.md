# Comparing `tmp/habapp_rules-2.1.1.tar.gz` & `tmp/habapp_rules-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habapp_rules-2.1.1.tar", last modified: Sat Feb  4 20:55:47 2023, max compression
+gzip compressed data, was "habapp_rules-3.0.0.tar", last modified: Fri Apr 28 21:01:52 2023, max compression
```

## Comparing `habapp_rules-2.1.1.tar` & `habapp_rules-3.0.0.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.496075 habapp_rules-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-04 20:55:47.496075 habapp_rules-2.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.492075 habapp_rules-2.1.1/habapp_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.492075 habapp_rules-2.1.1/habapp_rules/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/bridge/knx_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.492075 habapp_rules-2.1.1/habapp_rules/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/common/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/common/state_machine_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.496075 habapp_rules-2.1.1/habapp_rules/system/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/system/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/system/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/habapp_rules/system/summer_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:55:47.492075 habapp_rules-2.1.1/habapp_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-04 20:55:47.000000 habapp_rules-2.1.1/habapp_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-04 20:55:47.000000 habapp_rules-2.1.1/habapp_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 20:55:47.000000 habapp_rules-2.1.1/habapp_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-04 20:55:47.000000 habapp_rules-2.1.1/habapp_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-04 20:55:47.000000 habapp_rules-2.1.1/habapp_rules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 20:55:47.496075 habapp_rules-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-04 20:55:34.000000 habapp_rules-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.034219 habapp_rules-3.0.0/habapp_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27402 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/actors/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/actors/light_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/actors/state_observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/bridge/knx_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/common/hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/common/logic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/state_machine_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/core/timeout_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/habapp_rules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/system/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/system/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/habapp_rules/system/summer_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:01:52.034219 habapp_rules-3.0.0/habapp_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 21:01:51.000000 habapp_rules-3.0.0/habapp_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-28 21:01:52.000000 habapp_rules-3.0.0/habapp_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:01:51.000000 habapp_rules-3.0.0/habapp_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 21:01:51.000000 habapp_rules-3.0.0/habapp_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 21:01:51.000000 habapp_rules-3.0.0/habapp_rules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:01:52.038219 habapp_rules-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-28 21:01:41.000000 habapp_rules-3.0.0/setup.py
```

### Comparing `habapp_rules-2.1.1/LICENCE` & `habapp_rules-3.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `habapp_rules-2.1.1/habapp_rules/bridge/knx_mqtt.py` & `habapp_rules-3.0.0/habapp_rules/bridge/knx_mqtt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Rules for bridging KNX controller to MQTT items."""
 import logging
 
 import HABApp
 
-LOGGER = logging.getLogger(f"HABApp.{__name__}")
+import habapp_rules.core.logger
+
+LOGGER = logging.getLogger(__name__)
 
 
 class KnxMqttDimmerBridge(HABApp.Rule):
 	"""Create a bridge to control a MQTT dimmer from a KNX controller (e.g. wall switch).
 
 	To use this the items must be configured according the following example:
 	- knx_dimmer_ctr: autoupdate must be activated, thing:  [ switch="1/1/124+1/1/120", position="1/1/125+1/1/123", increaseDecrease="1/1/122" ] for switch/position: at first always use the RM-GA, second is the control-GA
@@ -21,14 +23,15 @@
 
 		:param knx_dimmer_ctr: name of KNX control item
 		:param mqtt_dimmer: name of MQTT item
 		:param increase_value: value which is set when INCREASE was received.
 		:param decrease_value: value which is set when DECREASE was received.
 		"""
 		HABApp.Rule.__init__(self)
+		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, f"{knx_dimmer_ctr}__{mqtt_dimmer}")
 
 		self.__increase_value = increase_value
 		self.__decrease_value = decrease_value
 
 		self._knx_item = HABApp.openhab.items.DimmerItem.get_item(knx_dimmer_ctr)
 		self._mqtt_item = HABApp.openhab.items.DimmerItem.get_item(mqtt_dimmer)
 
@@ -51,15 +54,15 @@
 				self._mqtt_item.oh_send_command(100)
 		elif event.value == "DECREASE":
 			if self._mqtt_item.value > self.__decrease_value:
 				self._mqtt_item.oh_send_command(self.__decrease_value)
 			else:
 				self._mqtt_item.oh_send_command(0)
 		else:
-			LOGGER.error(f"command '{event.value}' ist not supported!")
+			self._instance_logger.error(f"command '{event.value}' ist not supported!")
 
 	def _cb_mqtt_event(self, event: HABApp.openhab.events.ItemStateChangedEvent) -> None:
 		"""Callback, which is called if a MQTT state change event happens.
 
 		:param event: HABApp event
 		"""
 		self._knx_item.oh_post_update(event.value)
```

### Comparing `habapp_rules-2.1.1/habapp_rules/common/logic.py` & `habapp_rules-3.0.0/habapp_rules/common/logic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Implementations of logical functions."""
 import abc
 import logging
 
 import HABApp
 
-import habapp_rules.common.helper
+import habapp_rules.core.helper
+import habapp_rules.core.logger
 
-LOGGER = logging.getLogger(f"HABApp.{__name__}")
+LOGGER = logging.getLogger(__name__)
 
 
 class _Base(HABApp.Rule):
 	"""Base class for logical functions."""
 
 	def __init__(self, input_names: list[str], output_name: str) -> None:
 		"""Init a logical function.
 
 		:param input_names: list of input items (must be either Switch or Contact and all have to match to output_item)
 		:param output_name: name of output item
 		:raises TypeError: if unsupported item-type is given for output_name
 		"""
 		HABApp.Rule.__init__(self)
+		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, output_name)
 
 		self._output_item = HABApp.openhab.items.OpenhabItem.get_item(output_name)
 
 		if isinstance(self._output_item, HABApp.openhab.items.SwitchItem):
 			self._positive_state = "ON"
 			self._negative_state = "OFF"
 		elif isinstance(self._output_item, HABApp.openhab.items.ContactItem):
@@ -34,15 +36,15 @@
 
 		self._input_items = []
 		for name in input_names:
 			if isinstance(input_item := HABApp.openhab.items.OpenhabItem.get_item(name), type(self._output_item)):
 				self._input_items.append(input_item)
 				input_item.listen_event(self._cb_input_event, HABApp.openhab.events.ItemStateEventFilter())
 			else:
-				LOGGER.error(f"Item '{name}' must have the same type like the output item. Expected: {type(self._output_item)} | actual : {type(input_item)}")
+				self._instance_logger.error(f"Item '{name}' must have the same type like the output item. Expected: {type(self._output_item)} | actual : {type(input_item)}")
 
 		self._cb_input_event(None)
 
 	@abc.abstractmethod
 	def _cb_input_event(self, event: HABApp.openhab.events.ItemStateEvent | None) -> None:
 		"""Callback, which is called if one of the input items had a state event.
 
@@ -53,15 +55,15 @@
 		"""Set state to the output element
 
 		:param output_state: state which will be set
 		"""
 		if isinstance(self._output_item, HABApp.openhab.items.ContactItem):
 			self._output_item.oh_post_update(output_state)
 		else:
-			habapp_rules.common.helper.send_if_different(self._output_item.name, output_state)
+			habapp_rules.core.helper.send_if_different(self._output_item.name, output_state)
 
 
 class And(_Base):
 	"""Logical AND function."""
 
 	def _cb_input_event(self, event: HABApp.openhab.events.ItemStateEvent | None) -> None:
 		"""Callback, which is called if one of the input items had a state event.
```

### Comparing `habapp_rules-2.1.1/habapp_rules/system/presence.py` & `habapp_rules-3.0.0/habapp_rules/system/presence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 """Rule to detect presence or absence."""
 import logging
 import threading
-import typing
 
 import HABApp.openhab.definitions
 import HABApp.openhab.events
 import HABApp.openhab.interface
 import HABApp.openhab.items
 import HABApp.util
 
-import habapp_rules.common.helper
-import habapp_rules.common.state_machine_rule
+import habapp_rules.core.helper
+import habapp_rules.core.logger
+import habapp_rules.core.state_machine_rule
 
-LOGGER = logging.getLogger(f"HABApp.{__name__}")
-LOGGER.setLevel("DEBUG")
+LOGGER = logging.getLogger(__name__)
 
 
 # pylint: disable=no-member
-class Presence(habapp_rules.common.state_machine_rule.StateMachineRule):
-	"""Rules class to manage presence of a home."""
+class Presence(habapp_rules.core.state_machine_rule.StateMachineRule):
+	"""Rules class to manage presence of a home.
+
+	Hint: If you have some kind of guest-mode, use a guest-available switch as a phone to enable a persistent presence, also if all phones are not at home
+
+	Example OpenHAB configuration:
+	# KNX-things:
+	Thing device T00_99_OpenHab_Presence "KNX OpenHAB Presence"{
+        Type switch-control        : presence       "Presence"      [ ga="0/2/11+0/2/10"]
+        Type switch-control        : leaving        "Leaving"       [ ga="0/2/21+0/2/20"]
+    }
+
+    # Items:
+    Switch    I01_00_Presence    "Presence [%s]"    <presence>    (G00_00_rrd4j)    ["Status", "Presence"]    {channel="knx:device:bridge:T00_99_OpenHab_Presence:presence"}
+	Switch    I01_00_Leaving     "Leaving [%s]"     <leaving>                                                 {channel="knx:device:bridge:T00_99_OpenHab_Presence:leaving"}
+
+	# Rule init:
+	habapp_rules.system.presence.Presence("I01_00_Presence", "I01_00_Leaving")
+	"""
 
 	states = [
 		{"name": "presence"},
 		{"name": "leaving", "timeout": 5 * 60, "on_timeout": "absence_detected"},  # leaving takes 5 minutes
 		{"name": "absence", "timeout": 1.5 * 24 * 3600, "on_timeout": "long_absence_detected"},  # switch to long absence after 1.5 days
 		{"name": "long_absence"}
 	]
@@ -31,48 +47,55 @@
 		{"trigger": "presence_detected", "source": ["absence", "long_absence"], "dest": "presence"},
 		{"trigger": "leaving_detected", "source": ["presence", "absence", "long_absence"], "dest": "leaving"},
 		{"trigger": "abort_leaving", "source": "leaving", "dest": "presence"},
 		{"trigger": "absence_detected", "source": ["presence", "leaving"], "dest": "absence"},
 		{"trigger": "long_absence_detected", "source": "absence", "dest": "long_absence"},
 	]
 
-	def __init__(self, name_presence: str, outside_door_names: typing.List[str], leaving_name: str, state_name: str = None, phone_names: typing.List[str] = None) -> None:
+	def __init__(self, name_presence: str, leaving_name: str, outside_door_names: list[str] | None = None, phone_names: list[str] | None = None, state_name: str | None = None, state_label: str = "Presence state") -> None:
 		"""Init of Presence object.
 
 		:param name_presence: name of OpenHAB presence item
-		:param outside_door_names: list of names of OpenHAB outdoor door items
 		:param leaving_name: name of OpenHAB leaving item (SwitchItem)
-		:param state_name: name of OpenHAB item for storing the current state (StringItem)
+		:param outside_door_names: list of names of OpenHAB outdoor door items
 		:param phone_names: list of names of OpenHAB phone items
+		:param state_name: name of OpenHAB item for storing the current state (StringItem)
+		:param state_label: label of OpenHAB item for storing the current state (StringItem)
 		"""
-		super().__init__(state_name)
+		if not outside_door_names:
+			outside_door_names = []
+		if not phone_names:
+			phone_names = []
+
+		habapp_rules.core.state_machine_rule.StateMachineRule.__init__(self, state_name, state_label)
+		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, name_presence)
 
 		# init items
 		self.__presence_item = HABApp.openhab.items.SwitchItem.get_item(name_presence)
 		self.__leaving_item = HABApp.openhab.items.SwitchItem.get_item(leaving_name)
 		self.__outside_door_items = [HABApp.openhab.items.ContactItem.get_item(name) for name in outside_door_names]
 		self.__phone_items = [HABApp.openhab.items.SwitchItem.get_item(name) for name in phone_names]
 
 		# init state machine
-		self.state_machine = habapp_rules.common.state_machine_rule.StateMachineWithTimeout(
+		self.state_machine = habapp_rules.core.state_machine_rule.StateMachineWithTimeout(
 			model=self,
 			states=self.states,
 			transitions=self.trans,
 			ignore_invalid_triggers=True,
 			after_state_change="_update_openhab_state")
 		self._set_initial_state()
 
 		# add callbacks
 		self.__leaving_item.listen_event(self._cb_leaving, HABApp.openhab.events.ItemStateChangedEventFilter())
 		self.__presence_item.listen_event(self._cb_presence, HABApp.openhab.events.ItemStateChangedEventFilter())
 		HABApp.util.EventListenerGroup().add_listener(self.__outside_door_items, self._cb_outside_door, HABApp.core.events.ValueChangeEventFilter()).listen()
 		HABApp.util.EventListenerGroup().add_listener(self.__phone_items, self._cb_phone, HABApp.core.events.ValueChangeEventFilter()).listen()
 
-		self.__phone_absence_timer: threading.Timer = None
-		LOGGER.debug(f"Init of presence rule {self.rule_name} was successful. Initial state = {self.state}")
+		self.__phone_absence_timer: threading.Timer | None = None
+		self._instance_logger.debug(super().get_initial_log_message())
 
 	def _get_initial_state(self, default_value: str = "presence") -> str:
 		"""Get initial state of state machine.
 
 		:param default_value: default / initial state
 		:return: return correct state if it could be detected, if not return default value
 		"""
@@ -95,53 +118,53 @@
 			return "long_absence" if self._item_state.value == "long_absence" else "absence"
 
 		return default_value
 
 	def _update_openhab_state(self) -> None:
 		"""Extend _update_openhab state of base class to also update other OpenHAB items."""
 		super()._update_openhab_state()
-		LOGGER.info(f"Presence state changed to {self.state}")
+		self._instance_logger.info(f"Presence state changed to {self.state}")
 
 		# update presence item
 		target_value = "ON" if self.state in {"presence", "leaving"} else "OFF"
-		habapp_rules.common.helper.send_if_different(self.__presence_item.name, target_value)
+		habapp_rules.core.helper.send_if_different(self.__presence_item.name, target_value)
 
-		habapp_rules.common.helper.send_if_different(self.__leaving_item.name, "ON" if self.state == "leaving" else "OFF")
+		habapp_rules.core.helper.send_if_different(self.__leaving_item.name, "ON" if self.state == "leaving" else "OFF")
 
 	def _cb_outside_door(self, event: HABApp.openhab.events.ItemStateChangedEvent) -> None:
 		"""Callback, which is called if any outside door changed state.
 
 		:param event: state change event of door item
 		"""
 		if event.value == "OPEN" and self.state != "presence":
-			LOGGER.debug(f"Presence detected by door ({event.name})")
+			self._instance_logger.debug(f"Presence detected by door ({event.name})")
 			self.presence_detected()
 
 	def _cb_leaving(self, event: HABApp.openhab.events.ItemStateChangedEvent) -> None:
 		"""Callback, which is called if leaving item changed state.
 
 		:param event: Item state change event of leaving item
 		"""
 		if event.value == "ON" and self.state in {"presence", "absence", "long_absence"}:
-			LOGGER.debug("Start leaving through leaving switch")
+			self._instance_logger.debug("Start leaving through leaving switch")
 			self.leaving_detected()
 		if event.value == "OFF" and self.state == "leaving":
-			LOGGER.debug("Abort leaving through leaving switch")
+			self._instance_logger.debug("Abort leaving through leaving switch")
 			self.abort_leaving()
 
 	def _cb_presence(self, event: HABApp.openhab.events.ItemStateChangedEvent) -> None:
 		"""Callback, which is called if presence item changed state.
 
 		:param event: Item state change event of presence item
 		"""
 		if event.value == "ON" and self.state in {"absence", "long_absence"}:
-			LOGGER.debug("Presence was set manually by presence switch")
+			self._instance_logger.debug("Presence was set manually by presence switch")
 			self.presence_detected()
 		elif event.value == "OFF" and self.state in {"presence", "leaving"}:
-			LOGGER.debug("Absence was set manually by presence switch")
+			self._instance_logger.debug("Absence was set manually by presence switch")
 			self.absence_detected()
 
 	def _cb_phone(self, event: HABApp.openhab.events.ItemStateChangedEvent) -> None:
 		"""Callback, which is called if a phone state changed.
 
 		:param event: Item state change event of phone item
 		"""
@@ -149,21 +172,21 @@
 		if active_phones == 1 and event.value == "ON":
 			# first phone switched to ON
 			if self.__phone_absence_timer:
 				self.__phone_absence_timer.cancel()
 				self.__phone_absence_timer = None
 
 			if self.state in {"absence", "long_absence"}:
-				LOGGER.debug("Presence was set through first phone joined network")
+				self._instance_logger.debug("Presence was set through first phone joined network")
 				self.presence_detected()
 
 		elif active_phones == 0 and event.value == "OFF":
 			# last phone switched to OFF
 			self.__phone_absence_timer = threading.Timer(20 * 60, self.__set_leaving_through_phone)
 			self.__phone_absence_timer.start()
 
 	def __set_leaving_through_phone(self) -> None:
 		"""Set leaving detected if timeout expired."""
 		if self.state == "presence":
-			LOGGER.debug("Leaving was set, because last phone left some time ago.")
+			self._instance_logger.debug("Leaving was set, because last phone left some time ago.")
 			self.leaving_detected()
 		self.__phone_absence_timer = None
```

### Comparing `habapp_rules-2.1.1/habapp_rules/system/sleep.py` & `habapp_rules-3.0.0/habapp_rules/system/sleep.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,48 @@
 
 import HABApp.openhab.definitions
 import HABApp.openhab.events
 import HABApp.openhab.interface
 import HABApp.openhab.items
 import HABApp.util
 
-import habapp_rules.common.state_machine_rule
-import habapp_rules.common.helper
+import habapp_rules.core.helper
+import habapp_rules.core.logger
+import habapp_rules.core.state_machine_rule
 
-LOGGER = logging.getLogger(f"HABApp.{__name__}")
-LOGGER.setLevel("DEBUG")
+LOGGER = logging.getLogger(__name__)
 
 
 # pylint: disable=no-member
-class Sleep(habapp_rules.common.state_machine_rule.StateMachineRule):
-	"""Rules class to manage sleep state."""
+class Sleep(habapp_rules.core.state_machine_rule.StateMachineRule):
+	"""Rules class to manage sleep state.
+
+	Example OpenHAB configuration:
+	# KNX-things:
+	Thing device T00_99_OpenHab_Sleep "KNX OpenHAB Sleep"{
+        Type switch             : sleep             "Sleep Request"             [ ga="0/2/30"]
+        Type switch-control     : sleep_RM          "Sleep RM"                  [ ga="0/2/31"]
+
+        Type switch             : sleep_lock        "Sleep Lock Request"        [ ga="0/2/32"]
+        Type switch-control     : sleep_lock_RM     "Sleep Lock RM"             [ ga="0/2/33"]
+
+        Type string-control     : sleep_text        "Sleep Text"                [ ga="16.000:0/2/34"]
+    }
+
+    # Items:
+    Switch    I01_02_Sleep              "Sleep [%s]"                <moon>     {channel="knx:device:bridge:T00_99_OpenHab_Sleep:sleep_RM"}
+	Switch    I01_02_Sleep_req          "Sleep request"             <moon>     {channel="knx:device:bridge:T00_99_OpenHab_Sleep:sleep"}
+	String    I01_02_Sleep_text         "Text for display [%s]"                {channel="knx:device:bridge:T00_99_OpenHab_Sleep:sleep_text"}
+	Switch    I01_02_Sleep_lock         "Lock [%s]"                 <lock>     {channel="knx:device:bridge:T00_99_OpenHab_Sleep:sleep_lock_RM"}
+	Switch    I01_02_Sleep_lock_req     "Lock request"              <lock>     {channel="knx:device:bridge:T00_99_OpenHab_Sleep:sleep_lock"}
+	String    I01_02_Sleep_State        "State [%s]"                <state>
+
+	# Rule init:
+	habapp_rules.system.sleep.Sleep("I01_02_Sleep","I01_02_Sleep_req", "I01_02_Sleep_State", "I01_02_Sleep_lock", "I01_02_Sleep_lock_req", "I01_02_Sleep_text")
+	"""
 
 	states = [
 		{"name": "awake"},
 		{"name": "pre_sleeping", "timeout": 3, "on_timeout": "pre_sleeping_timeout"},
 		{"name": "sleeping"},
 		{"name": "post_sleeping", "timeout": 3, "on_timeout": "post_sleeping_timeout"},
 		{"name": "locked"},
@@ -34,53 +58,56 @@
 		{"trigger": "end_sleeping", "source": "pre_sleeping", "dest": "locked", "conditions": "lock_request_active"},
 		{"trigger": "post_sleeping_timeout", "source": "post_sleeping", "dest": "awake", "unless": "lock_request_active"},
 		{"trigger": "post_sleeping_timeout", "source": "post_sleeping", "dest": "locked", "conditions": "lock_request_active"},
 		{"trigger": "set_lock", "source": "awake", "dest": "locked"},
 		{"trigger": "release_lock", "source": "locked", "dest": "awake"}
 	]
 
-	def __init__(self, name_sleep: str, name_sleep_request: str, state_name: str = None, name_lock: str = None, name_lock_request: str = None, name_display_text: str = None) -> None:
+	def __init__(self, name_sleep: str, name_sleep_request: str, name_lock: str = None, name_lock_request: str = None, name_display_text: str = None, state_name: str = None, state_label: str = "Sleep state") -> None:
 		"""Init of Sleep object.
 
 		:param name_sleep: name of OpenHAB sleep item (SwitchItem)
 		:param name_sleep_request: name of OpenHAB sleep request item (SwitchItem)
-		:param state_name: name of OpenHAB item for storing the current state (StringItem)
 		:param name_lock: name of OpenHAB lock item (SwitchItem)
 		:param name_lock_request: name of OpenHAB lock request item (SwitchItem)
 		:param name_display_text: name of OpenHAB display text item (StringItem)
+		:param state_name: name of OpenHAB item for storing the current state (StringItem)
+		:param state_label: label of OpenHAB item for storing the current state (StringItem)
 		"""
-		super().__init__(state_name)
+		habapp_rules.core.state_machine_rule.StateMachineRule.__init__(self, state_name, state_label)
+		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, name_sleep)
 
 		# init items
 		self.__item_sleep = HABApp.openhab.items.SwitchItem.get_item(name_sleep)
 		self.__item_sleep_request = HABApp.openhab.items.SwitchItem.get_item(name_sleep_request)
 		self.__item_lock = HABApp.openhab.items.SwitchItem.get_item(name_lock) if name_lock else None
 		self.__item_lock_request = HABApp.openhab.items.SwitchItem.get_item(name_lock_request) if name_lock_request else None
 		self.__item_display_text = HABApp.openhab.items.StringItem.get_item(name_display_text) if name_display_text else None
 
 		# init attributes
 		self._sleep_request_active = bool(self.__item_sleep_request)
 		self._lock_request_active = bool(self.__item_lock_request) if self.__item_lock_request is not None else False
 
 		# init state machine
-		self.state_machine = habapp_rules.common.state_machine_rule.StateMachineWithTimeout(
+		self.state_machine = habapp_rules.core.state_machine_rule.StateMachineWithTimeout(
 			model=self,
 			states=self.states,
 			transitions=self.trans,
 			ignore_invalid_triggers=True,
 			after_state_change="_update_openhab_state")
 		self._set_initial_state()
 
 		self._update_openhab_state()
 
 		# add callbacks
 		self.__item_sleep_request.listen_event(self._cb_sleep_request, HABApp.openhab.events.ItemStateChangedEventFilter())
 		if self.__item_lock_request is not None:
 			self.__item_lock_request.listen_event(self._cb_lock_request, HABApp.openhab.events.ItemStateChangedEventFilter())
-		LOGGER.debug(f"Init of sleep rule {self.rule_name} was successful. Initial state = {self.state}")
+
+		self._instance_logger.debug(super().get_initial_log_message())
 
 	def _get_initial_state(self, default_value: str = "awake") -> str:
 		"""Get initial state of state machine.
 
 		:param default_value: default / initial state
 		:return: return correct state if it could be detected, if not return default value
 		"""
@@ -114,17 +141,17 @@
 
 	def _update_openhab_state(self):
 		"""Extend _update_openhab state of base class to also update other OpenHAB items."""
 		super()._update_openhab_state()
 
 		# update sleep state
 		if self.state in {"pre_sleeping", "sleeping"}:
-			habapp_rules.common.helper.send_if_different(self.__item_sleep.name, "ON")
+			habapp_rules.core.helper.send_if_different(self.__item_sleep.name, "ON")
 		else:
-			habapp_rules.common.helper.send_if_different(self.__item_sleep.name, "OFF")
+			habapp_rules.core.helper.send_if_different(self.__item_sleep.name, "OFF")
 
 		# update lock state
 		self.__update_lock_state()
 
 		# update display text
 		if self.__item_display_text is not None:
 			self.__item_display_text.oh_send_command(self.__get_display_text())
@@ -146,32 +173,32 @@
 			return "Gesperrt"
 		return ""
 
 	def __update_lock_state(self):
 		"""Update the return lock state value of OpenHAB item."""
 		if self.__item_lock is not None:
 			if self.state in {"pre_sleeping", "post_sleeping", "locked"}:
-				habapp_rules.common.helper.send_if_different(self.__item_lock.name, "ON")
+				habapp_rules.core.helper.send_if_different(self.__item_lock.name, "ON")
 			else:
-				habapp_rules.common.helper.send_if_different(self.__item_lock.name, "OFF")
+				habapp_rules.core.helper.send_if_different(self.__item_lock.name, "OFF")
 
 	def _cb_sleep_request(self, event: HABApp.openhab.events.ItemStateChangedEvent):
 		"""Callback, which is called if sleep request item changed state.
 
 		:param event: Item state change event of sleep_request item
 		"""
 		if event.value == "ON" and self.state == "awake":
-			LOGGER.debug("Start sleeping through sleep switch")
+			self._instance_logger.debug("Start sleeping through sleep switch")
 			self._sleep_request_active = True
 			self.start_sleeping()
 		elif event.value == "ON" and self.state == "locked":
 			self._sleep_request_active = False
 			self.__item_sleep_request.oh_send_command("OFF")
 		elif event.value == "OFF" and self.state in {"sleeping", "pre_sleeping"}:
-			LOGGER.debug("End sleeping through sleep switch")
+			self._instance_logger.debug("End sleeping through sleep switch")
 			self._sleep_request_active = True
 			self.end_sleeping()
 
 	def _cb_lock_request(self, event: HABApp.openhab.events.ItemStateChangedEvent):
 		"""Callback, which is called if lock request item changed state.
 
 		:param event: Item state change event of sleep_request item
```

### Comparing `habapp_rules-2.1.1/habapp_rules/system/summer_winter.py` & `habapp_rules-3.0.0/habapp_rules/system/summer_winter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Rule to detect whether it is summer or winter."""
-import collections
 import datetime
 import logging
 import statistics
 
 import HABApp
 
-LOGGER = logging.getLogger(f"HABApp.{__name__}")
+import habapp_rules.common.hysteresis
+import habapp_rules.core.logger
+
+LOGGER = logging.getLogger(__name__)
 
 
 class SummerWinterException(Exception):
 	"""Custom Exception for SummerWinter"""
 
 
 class SummerWinter(HABApp.Rule):
@@ -22,39 +24,33 @@
 		:param outside_temperature_name: Name of outside temperature item. OpenHAB-Type must be Number item
 		:param summer_name: Name of summer item. OpenHAB-Type must be Switch item
 		:param persistence_service: Name of persistence service
 		:param days: number of days in the past which will be used to check if it is summer
 		:param temperature_threshold: threshold weighted temperature for summer
 		:param last_check_name: Name of last check item. OpenHAB-Type must be DateTime item
 		"""
-		super().__init__()
+		HABApp.Rule.__init__(self)
+		self._instance_logger = habapp_rules.core.logger.InstanceLogger(LOGGER, summer_name)
 
 		# set class variables
 		self._persistence_service = persistence_service
 		self._days = days
-		self._temperature_threshold = temperature_threshold
+		self._hysteresis_switch = habapp_rules.common.hysteresis.HysteresisSwitch(temperature_threshold, 0.5)
 		self.__now = datetime.datetime.now()
 
 		# get items
 		self._outside_temp_item = HABApp.openhab.items.NumberItem.get_item(outside_temperature_name)
 		self._item_summer = HABApp.openhab.items.SwitchItem.get_item(summer_name)
 		self._item_last_check = HABApp.openhab.items.DatetimeItem.get_item(last_check_name) if last_check_name else None
 
 		# run at init and every day at 23:00
 		self.run.soon(self._cb_update_summer)
 		self.run.on_every_day(datetime.time(23), self._cb_update_summer)
 
-	def __get_threshold_with_hysteresis(self) -> float:
-		"""Getting threshold with hysteresis to avoid toggling of summer / winter.
-
-		:return: temperature threshold with hysteresis depending on summer / winter
-		"""
-		if bool(self._item_summer):
-			return self._temperature_threshold - 0.5
-		return self._temperature_threshold
+		LOGGER.debug("Init of Summer / Winter successful")
 
 	def __get_weighted_mean(self, days_in_past: int) -> float:
 		"""Get weighted mean temperature.
 
 		The weighted mean temperature will be calculated according the following formula: (T07 + T14 + T22 + T22) / 4 where T07 is the temperature at 7:00 (and so on)
 		It is possible to get the weighted temperature of today or of some days in the past -> defined by the days_in past attribute. If this method is called before 22:00 there will be an offset of one day.
 		:param days_in_past: if days in past is set to 0 it will return the mean of today. 1 will return the offset of yesterday
@@ -65,57 +61,53 @@
 		if self.__now.hour < 23:
 			day_offset = 1
 
 		temperature_values = []
 		for hour in [7, 14, 22]:
 			start_time = datetime.datetime(self.__now.year, self.__now.month, self.__now.day, hour, 0) - datetime.timedelta(days=day_offset + days_in_past)
 			end_time = start_time + datetime.timedelta(hours=1)
-			values = self._outside_temp_item.get_persistence_data(persistence=self._persistence_service, start_time=start_time, end_time=end_time)
-			values_sorted = collections.OrderedDict(sorted(values.get_data().items()))
-			if not values_sorted:
-				raise SummerWinterException(f"No data for days_in_past = {days_in_past} and hour = {hour}")
-			temperature_values.append(list(values_sorted.values())[0])
+			persistence_data = self._outside_temp_item.get_persistence_data(persistence=self._persistence_service, start_time=start_time, end_time=end_time)
+			if not persistence_data.data:
+				raise SummerWinterException(f"No data for {start_time}")
+			temperature_values.append(next(iter(persistence_data.data.values())))
 		return (sum(temperature_values) + temperature_values[2]) / 4
 
 	def __is_summer(self) -> bool:
 		"""Check if it is summer (or winter).
 
 		:return: Returns True if it is summer.
 		:raises SummerWinterException: if summer/winter could not be detected
 		"""
 		self.__now = datetime.datetime.now()
 		values = []
 		for day in range(self._days):
 			try:
 				values.append(self.__get_weighted_mean(day))
 			except SummerWinterException:
-				LOGGER.warning(f"Could not get mean value of day -{day}")
-
-		if len(values) <= self._days * 0.5:
-			raise SummerWinterException(f"Not enough values to detect summer/winter. Expected: {self._days} | actual: {len(values)}")
+				self._instance_logger.warning(f"Could not get mean value of day -{day}")
 
-		is_summer = False
-		if (mean_value := statistics.mean(values)) > (threshold := self.__get_threshold_with_hysteresis()):
-			is_summer = True
+		if not values:
+			raise SummerWinterException("Not enough data to detect summer/winter")
 
-		LOGGER.debug(f"Check Summer/Winter. values = {values} | mean = {mean_value} | threshold = {threshold} | summer = {is_summer}")
+		is_summer = self._hysteresis_switch.get_output(mean_value := statistics.mean(values))
+		self._instance_logger.debug(f"Check Summer/Winter. values = {values} | mean = {mean_value} | summer = {is_summer}")
 		return is_summer
 
 	def _cb_update_summer(self) -> None:
 		"""Callback to update the summer item."""
 		try:
 			is_summer = self.__is_summer()
 		except SummerWinterException:
-			LOGGER.exception("Could not get summer / winter")
+			self._instance_logger.error("Could not get summer / winter")
 			return
 
 		# get target state of summer
 		target_value = "ON" if is_summer else "OFF"
 
 		# send state
 		if self._item_summer.value != target_value:
 			self._item_summer.oh_send_command(target_value)
-			LOGGER.info(f"Summer changed to {target_value}")
+			self._instance_logger.info(f"Summer changed to {target_value}")
 
 		# update last update item at every call
 		if self._item_last_check:
 			self._item_last_check.oh_send_command(datetime.datetime.now())
```

### Comparing `habapp_rules-2.1.1/habapp_rules.egg-info/SOURCES.txt` & `habapp_rules-3.0.0/habapp_rules.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,28 @@
 habapp_rules/__init__.py
 habapp_rules/__version__.py
 habapp_rules.egg-info/PKG-INFO
 habapp_rules.egg-info/SOURCES.txt
 habapp_rules.egg-info/dependency_links.txt
 habapp_rules.egg-info/requires.txt
 habapp_rules.egg-info/top_level.txt
+habapp_rules/actors/__init__.py
+habapp_rules/actors/light.py
+habapp_rules/actors/light_config.py
+habapp_rules/actors/state_observer.py
 habapp_rules/bridge/__init__.py
 habapp_rules/bridge/knx_mqtt.py
 habapp_rules/common/__init__.py
-habapp_rules/common/helper.py
+habapp_rules/common/hysteresis.py
 habapp_rules/common/logic.py
-habapp_rules/common/state_machine_rule.py
+habapp_rules/core/__init__.py
+habapp_rules/core/exceptions.py
+habapp_rules/core/helper.py
+habapp_rules/core/logger.py
+habapp_rules/core/state_machine_rule.py
+habapp_rules/core/timeout_list.py
+habapp_rules/sensors/__init__.py
+habapp_rules/sensors/motion.py
 habapp_rules/system/__init__.py
 habapp_rules/system/presence.py
 habapp_rules/system/sleep.py
 habapp_rules/system/summer_winter.py
```

### Comparing `habapp_rules-2.1.1/setup.py` & `habapp_rules-3.0.0/setup.py`

 * *Files identical despite different names*

