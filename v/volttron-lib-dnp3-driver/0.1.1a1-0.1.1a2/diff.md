# Comparing `tmp/volttron_lib_dnp3_driver-0.1.1a1.tar.gz` & `tmp/volttron_lib_dnp3_driver-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a1.tar", max compression
+gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a2.tar", max compression
```

## Comparing `volttron_lib_dnp3_driver-0.1.1a1.tar` & `volttron_lib_dnp3_driver-0.1.1a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11928 2023-04-17 16:47:29.343659 volttron_lib_dnp3_driver-0.1.1a1/LICENSE
--rw-r--r--   0        0        0    20538 2023-04-17 16:47:29.343659 volttron_lib_dnp3_driver-0.1.1a1/README.md
--rw-r--r--   0        0        0     1566 2023-04-17 16:49:31.212411 volttron_lib_dnp3_driver-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 16:47:29.343659 volttron_lib_dnp3_driver-0.1.1a1/src/volttron/driver/interfaces/dnp3/__init__.py
--rw-r--r--   0        0        0     8832 2023-04-17 16:47:29.343659 volttron_lib_dnp3_driver-0.1.1a1/src/volttron/driver/interfaces/dnp3/dnp3.py
--rw-r--r--   0        0        0    22231 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a1/setup.py
--rw-r--r--   0        0        0    21656 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0    20538 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/README.md
+-rw-r--r--   0        0        0     1584 2023-04-28 17:39:27.532901 volttron_lib_dnp3_driver-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/__init__.py
+-rw-r--r--   0        0        0     9189 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/dnp3.py
+-rw-r--r--   0        0        0    22231 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a2/setup.py
+-rw-r--r--   0        0        0    21656 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a2/PKG-INFO
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/LICENSE` & `volttron_lib_dnp3_driver-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/README.md` & `volttron_lib_dnp3_driver-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/pyproject.toml` & `volttron_lib_dnp3_driver-0.1.1a2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "volttron-lib-dnp3-driver"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "A minimal implementation of a driver for the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 keywords = []
@@ -30,14 +30,15 @@
 volttron-lib-base-driver = "^0.2.0rc0"
 dnp3-python = "^0.2.3b2"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.4.0rc0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
+pytest-env = ">0"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
 mypy = "^0.942"
 coverage = "^6.3.2"
 isort = "^5.10.1"
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/src/volttron/driver/interfaces/dnp3/dnp3.py` & `volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/dnp3.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,27 +42,28 @@
 
 # Type alias
 RegisterValue = Union[int, str, float, bool]
 Register = TypeVar("Register", bound=BaseRegister)
 
 
 class Dnp3Register(BaseRegister):
+    # TODO: developed more robust logic when not connecting with an outstation.
 
     def __init__(self, read_only, pointName, units, reg_type, default_value=None, description='',
                  reg_definition=None, master_application=None):
         # Note: the most important arguments are regDef and master_application
         # read_only determine whether the set_point logic can be implemented
         # (associated with "Writable" field in config-csv)
         # (Keep other arguments by following fake driver example convention)
         self.reg_def = reg_definition
         self.master_application = master_application
         self.reg_type = reg_type
         self.pointName = pointName
 
-        self.value = None
+        self._value = None  # use _value as cache
         self.group = int(reg_definition.get("Group"))
         self.variation = int(reg_definition.get("Variation"))
         self.index = int(reg_definition.get("Index"))
 
         super().__init__("byte", read_only, pointName, units, description='')
 
     @property
@@ -72,17 +73,18 @@
                                             group=self.group,
                                             variation=self.variation,
                                             index=self.index)
             if value is None:
                 _log.warning(f"Register value for pointName {self.pointName} is None.")
                 # raise ValueError(f"Register value for pointName {self.pointName} is None. Hence not publish.")
                 # TODO: figure out an elegant way to not publish None values.
-            return value
+            self._value = value
+            return self._value
         except Exception as e:
-            _log.error(e)
+            _log.exception(e, stack_info=True)
             _log.warning("udd_dnp3 driver (master) couldn't get value from the outstation.")
 
     @staticmethod
     def _get_outstation_pt(master_application, group, variation, index) -> RegisterValue:
         """
         Core logic to retrieve register value by polling a dnp3 outstation
         Note: using def get_db_by_group_variation_index
@@ -98,16 +100,17 @@
     def value(self, _val):
         try:
             self._set_outstation_pt(master_application=self.master_application,
                                     group=self.group,
                                     variation=self.variation,
                                     index=self.index,
                                     set_value=_val)
+            self._value = _val
         except Exception as e:
-            _log.error(e)
+            _log.exception(e, stack_info=True)
             _log.warning("udd_dnp3 driver (master) couldn't set value for the outstation.")
 
     @staticmethod
     def _set_outstation_pt(master_application, group, variation, index, set_value) -> None:
         """
         Core logic to send point operate command to outstation
         Note: using def send_direct_point_command
@@ -146,27 +149,29 @@
         register: Dnp3Register = self.get_register_by_name(point_name)
 
         return register.value
 
     def _set_point(self, point_name, value: RegisterValue):
         register: Dnp3Register = self.get_register_by_name(point_name)
         if register.read_only:
-            raise RuntimeError("Trying to write to a point configured read only: " + point_name)
+            raise ValueError("Trying to write to a point configured read only: " + point_name)
         # register.value = register.reg_type(value)  # old logic to cast value to reg_type value (not robust)
         register.value = value
-        # Note: simple retry logic
-        retry_max = 10
-        for n in range(retry_max):
-            if register.value == value:
-                return register.value
-            register.value = value
-            sleep(1)
-            # _log.info(f"Starting set_point {n}th RETRY for {point_name}")
-        _log.warning(f"Failed to set_point for {point_name} after {retry_max} retry.")
-        return None
+        return register._value
+        # # Note: simple retry logic
+        # # TODO: make retry attempt configurable
+        # retry_max = 3
+        # for n in range(retry_max):
+        #     if register._value == value:  # use _value as cache
+        #         return register.value
+        #     register.value = value  # otherwise, retry
+        #     sleep(1)
+        #     # _log.info(f"Starting set_point {n}th RETRY for {point_name}")
+        # _log.warning(f"Failed to set_point for {point_name} after {retry_max} retry.")
+        # return None
 
     def _scrape_all(self):
         result = {}
         read_registers = self.get_registers_by_type("byte", True)
         write_registers = self.get_registers_by_type("byte", False)
         for register in read_registers + write_registers:
             result[register.point_name] = register.value
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/setup.py` & `volttron_lib_dnp3_driver-0.1.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dnp3-python>=0.2.3b2,<0.3.0', 'volttron-lib-base-driver>=0.2.0rc0,<0.3.0']
 
 setup_kwargs = {
     'name': 'volttron-lib-dnp3-driver',
-    'version': '0.1.1a1',
+    'version': '0.1.1a2',
     'description': 'A minimal implementation of a driver for the VOLTTRON platform.',
     'long_description': '# volttron-lib-dnp3-driver\n\n[//]: # (TODO: get the badges)\n\nDistributed Network Protocol (DNP\nor [DNP3](https://en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance since its introduction in 1993. This\nprotocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of\ncritical infrastructure status, allowing for reliable remote control.\n\nDNP3 is typically used between centrally located masters and distributed remotes. The master provides the interface\nbetween the human network manager and the monitoring system. The remote (RTUs and intelligent electronic devices)\nprovides the interface between the master and the physical device(s) being monitored and/or controlled.\nThe DNP3-Driver is a wrapper on the DNP3 master following\nthe [VOLTTRON driver framework](https://volttron.readthedocs.io/en/develop/agent-framework/driver-framework/drivers-overview.html#driver-framework).\n\nNote that the DNP3-Driver requires a DNP3 outstation instance to properly function. e.g., polling data, setting point\nvalues, etc. The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can provide the essential outstation\nfunctionality, and as part of the DNP3-Driver dependency, it is immediately available after the DNP3-Driver is\ninstalled.\n\n# Prerequisites\n\n* Python 3 (tested with Python3.8, Python3.9, Python3.10)\n\n## Python\n\n<details>\n<summary>To install specific Python version (e.g., Python 3.8), we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>\n\n```shell\n# install pyenv\ngit clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup pyenv (you should also put these three lines in .bashrc or similar)\nexport PATH="${HOME}/.pyenv/bin:${PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$(pyenv init -)"\n\n# install Python 3.8\npyenv install 3.8.10\n\n# make it available globally\npyenv global system 3.8.10\n```\n\n</details>\n\n# Quick Start\n\nThe following recipe walks through the steps to install and configure a DNP3 Driver. Note that it uses default setup to\nwork out-of-the-box. Please feel free to refer to related documentations for details.\n\n1. Create and activate a virtual environment.\n\n   It is recommended to use a virtual environment for installing volttron.\n\n    ```shell\n    python -m venv env\n    source env/bin/activate\n    \n    pip install volttron\n    ```\n\n1. Install volttron and start the platform.\n\n   > **Note**:\n   > According to [volttron-core#readme](https://github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME\n   > environment variable is mandatory:\n\n   > ... if you have/had in the past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME\n   > $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of\n   > VOLTTRON(version 8.3 or earlier)\n\n    ```shell\n    # Setup enviornment variable\n    export VOLTTRON_HOME=/path/to/volttron_home/dir\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n1. Install the volttron platform driver:\n\n   Note: for reproducibility, this demo will install platform driver with `vip-identity==platform_driver_for_dnp3`.\n   Free feel to specify any agent vip-identity as desired.\n\n    ```shell\n    vctl install volttron-platform-driver --vip-identity platform_driver_for_dnp3 --start\n    ```\n\n    <details>\n    <summary>Verify with `vctl status`.</summary>\n\n    ```shell\n    (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ vctl status\n    \n    UUID   AGENT                             IDENTITY                     TAG PRIORITY STATUS          HEALTH                                   \n    \n    5      volttron-platform-driver-0.2.0rc1 platform_driver_for_dnp3                  running [23217] GOOD\n    ```\n\n    </details>\n\n1. Install the "volttron-lib-dnp3-driver" library.\n\n   There are two options to install the DNP3 Driver. You can install this library using the version on PyPi or install\n   it from the source code (`git clone` might be required.)\n\n    ```shell\n    # option 1: install from pypi\n    pip install volttron-lib-dnp3-driver\n    \n    # option 2: install from the source code\n    pip install <path-to-the-source-code-root>/volttron-lib-dnp3-driver/\n    ```\n\n1. Install a DNP3 Driver onto the Platform Driver.\n\n   Installing a DNP3 driver in the Platform Driver Agent requires adding copies of the device configuration and registry\n   configuration files to the Platform Driver’s configuration store. For demo purpose, we will use default configure\n   files.\n\n   Prepare the default config files:\n\n    ```shell\n    # Create config file place holders\n    mkdir config\n    touch config/dnp3-config.json\n    touch config/dnp3.csv\n    ```\n\n   Edit the `dnp3-config.json` as follows:\n\n    ```json\n    {\n      "driver_config": {\n        "master_ip": "0.0.0.0",\n        "outstation_ip": "127.0.0.1",\n        "master_id": 2,\n        "outstation_id": 1,\n        "port": 20000\n      },\n      "registry_config": "config://dnp3.csv",\n      "driver_type": "dnp3",\n      "interval": 5,\n      "timezone": "UTC",\n      "publish_depth_first_all": true,\n      "heart_beat_point": "random_bool"\n    }\n    ```\n\n   Edit the `dnp3.csv` as follows:\n\n    ```csv\n    Point Name,Volttron Point Name,Group,Variation,Index,Scaling,Units,Writable,Notes\n    AnalogInput_index0,AnalogInput_index0,30,6,0,1,NA,FALSE,Double Analogue input without status\n    AnalogInput_index1,AnalogInput_index1,30,6,1,1,NA,FALSE,Double Analogue input without status\n    AnalogInput_index2,AnalogInput_index2,30,6,2,1,NA,FALSE,Double Analogue input without status\n    AnalogInput_index3,AnalogInput_index3,30,6,3,1,NA,FALSE,Double Analogue input without status\n    BinaryInput_index0,BinaryInput_index0,1,2,0,1,NA,FALSE,Single bit binary input with status\n    BinaryInput_index1,BinaryInput_index1,1,2,1,1,NA,FALSE,Single bit binary input with status\n    BinaryInput_index2,BinaryInput_index2,1,2,2,1,NA,FALSE,Single bit binary input with status\n    BinaryInput_index3,BinaryInput_index3,1,2,3,1,NA,FALSE,Single bit binary input with status\n    AnalogOutput_index0,AnalogOutput_index0,40,4,0,1,NA,TRUE,Double-precision floating point with flags\n    AnalogOutput_index1,AnalogOutput_index1,40,4,1,1,NA,TRUE,Double-precision floating point with flags\n    AnalogOutput_index2,AnalogOutput_index2,40,4,2,1,NA,TRUE,Double-precision floating point with flags\n    AnalogOutput_index3,AnalogOutput_index3,40,4,3,1,NA,TRUE,Double-precision floating point with flags\n    BinaryOutput_index0,BinaryOutput_index0,10,2,0,1,NA,TRUE,Binary Output with flags\n    BinaryOutput_index1,BinaryOutput_index1,10,2,1,1,NA,TRUE,Binary Output with flags\n    BinaryOutput_index2,BinaryOutput_index2,10,2,2,1,NA,TRUE,Binary Output with flags\n    BinaryOutput_index3,BinaryOutput_index3,10,2,3,1,NA,TRUE,Binary Output with flags\n    \n    ```\n\n   Add config to the configuration store:\n\n    ```\n    vctl config store platform_driver_for_dnp3 devices/campus/building/dnp3 config/dnp3-config.json\n    vctl config store platform_driver_for_dnp3 dnp3.csv config/dnp3.csv --csv\n    ```\n\n    <details>\n    <summary>Verify with `vctl config list` and `vctl config get` command. \n    (Please refer to the `vctl config` documentation for more details.)</summary>\n\n    ```shell\n    (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ vctl config get platform_driver_for_dnp3 devices/campus/building/dnp3\n    {\n      "driver_config": {\n        "master_ip": "0.0.0.0",\n        "outstation_ip": "127.0.0.1",\n        "master_id": 2,\n        "outstation_id": 1,\n        "port": 20000\n      },\n      "registry_config": "config://dnp3.csv",\n      "driver_type": "dnp3",\n      "interval": 5,\n      "timezone": "UTC",\n      "publish_depth_first_all": true,\n      "heart_beat_point": "random_bool"\n    }\n    \n    (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ vctl config get platform_driver_for_dnp3 dnp3.csv\n    [\n      {\n        "Point Name": "AnalogInput_index0",\n        "Volttron Point Name": "AnalogInput_index0",\n        "Group": "30",\n        "Variation": "6",\n        "Index": "0",\n    ...\n    ]\n    ```\n\n    </details>\n\n1. Verify with logging data\n\n   When the DNP3-Driver is properly installed and configured, we can verify with logging data in "volttron.log".\n\n    ```\n    tail -f <path to folder containing volttron.log>/volttron.log\n    ```\n\n    <details>\n    <summary>Expected logging example</summary>\n\n    ```shell\n    ...\n    2023-03-13 23:26:56,611 (volttron-platform-driver-0.2.0rc1 23666) volttron.driver.base.driver(334) DEBUG: finish publishing: devices/campus/building/dnp3/all\n    2023-03-13 23:26:57,897 () volttron.services.auth.auth_service(235) DEBUG: after getting peerlist to send auth updates\n    2023-03-13 23:26:57,897 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform.control\n    2023-03-13 23:26:57,897 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform_driver_for_dnp3\n    2023-03-13 23:26:57,898 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform.health\n    2023-03-13 23:26:57,898 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform.config_store\n    2023-03-13 23:26:57,898 () volttron.services.auth.auth_service(193) INFO: auth file /home/kefei/.volttron/auth.json loaded\n    2023-03-13 23:26:57,898 () volttron.services.auth.auth_service(172) INFO: loading auth file /home/kefei/.volttron/auth.json\n    2023-03-13 23:26:57,898 () volttron.services.auth.auth_service(185) DEBUG: Sending auth updates to peers\n    2023-03-13 23:26:58,241 (volttron-platform-driver-0.2.0rc1 23666) <stdout>(0) INFO: [\'ms(1678768018241) INFO    tcpclient - Connecting to: 127.0.0.1\']\n    2023-03-13 23:26:58,241 (volttron-platform-driver-0.2.0rc1 23666) <stdout>(0) INFO: [\'ms(1678768018241) WARN    tcpclient - Error Connecting: Connection refused\']\n    2023-03-13 23:26:59,905 () volttron.services.auth.auth_service(235) DEBUG: after getting peerlist to send auth updates\n    2023-03-13 23:26:59,905 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform.control\n    2023-03-13 23:26:59,905 () volttron.services.auth.auth_service(239) DEBUG: Sending auth update to peers platform_driver_for_dnp3...\n    ]\n    ```\n    </details>\n\n1. (Optional) Verify with published data polled from outstation\n\n   To see data being polled from an outstation and published to the bus, we need to\n\n    * Set up an outstation, and\n    * install a [Listener Agent](https://pypi.org/project/volttron-listener/):\n\n   **Set up an outstation**: The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) is part of the dnp3-driver\n   dependency, and it is immediately available after the DNP3-Driver is installed.\n\n   **Open another terminal**, and run `dnp3demo outstation`. For demo purpose, we assign arbitrary values to the\n   point. (\n   More details about the "dnp3demo" module, please\n   see [dnp3demo-Module.md](https://github.com/VOLTTRON/dnp3-python/blob/main/docs/dnp3demo-Module.md))\n\n   ```shell\n    ==== Outstation Operation MENU ==================================\n    <ai> - update analog-input point value (for local reading)\n    <ao> - update analog-output point value (for local control)\n    <bi> - update binary-input point value (for local reading)\n    <bo> - update binary-output point value (for local control)\n    <dd> - display database\n    <dc> - display configuration\n    =================================================================\n   \n    ======== Your Input Here: ==(outstation)======\n    ai\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    0.1212 0\n    {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    1.2323 1\n    {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n   ```\n    <details>\n    <summary>Example of interaction with the `dnp3demo outstation` sub-command</summary>\n\n    ```shell\n    (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ dnp3demo outstation\n    dnp3demo.run_outstation {\'command\': \'outstation\', \'outstation_ip=\': \'0.0.0.0\', \'port=\': 20000, \'master_id=\': 2, \'outstation_id=\': 1}\n    ms(1678770551216) INFO    manager - Starting thread (0)\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n    ms(1678770551216) INFO    server - Listening on: 0.0.0.0:20000\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n    2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n    Connection error.\n    Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n    Start retry...\n    Connection error.\n    Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n    ms(1678770565247) INFO    server - Accepted connection from: 127.0.0.1\n    ==== Outstation Operation MENU ==================================\n    <ai> - update analog-input point value (for local reading)\n    <ao> - update analog-output point value (for local control)\n    <bi> - update binary-input point value (for local reading)\n    <bo> - update binary-output point value (for local control)\n    <dd> - display database\n    <dc> - display configuration\n    =================================================================\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    ai\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    0.1212 0\n    {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    1.2323 1\n    {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n    \n    \n    ======== Your Input Here: ==(outstation)======\n    ```\n    </details>\n\n   **Install the [Listener Agent](https://pypi.org/project/volttron-listener/)**:\n   Run `vctl install volttron-listener --start`. Once installed, you should see the data being published by viewing the\n   Volttron logs file. (i.e., `tail -f <path to folder containing volttron.log>/volttron.log`)\n   > **Note**:\n   > it is recommended to restart the Platform Driver after a specific driver is installed and configured. i.e.,\n   > using the `vctl restart <agent-uuid>` command.) The expected logging will be similar as follows:\n\n    ```shell\n    2023-03-14 00:11:55,000 (volttron-platform-driver-0.2.0rc0 24737) volttron.driver.base.driver(277) DEBUG: scraping device: campus/building/dnp3\n    2023-03-14 00:11:55,805 (volttron-platform-driver-0.2.0rc0 24737) volttron.driver.base.driver(330) DEBUG: publishing: devices/campus/building/dnp3/all\n    2023-03-14 00:11:55,810 (volttron-listener-0.2.0rc0 24424) listener.agent(104) INFO: Peer: pubsub, Sender: platform_driver_for_dnp3:, Bus: , Topic: devices/campus/building/dnp3/all, Headers: {\'Date\': \'2023-03-14T05:11:55.805245+00:00\', \'TimeStamp\': \'2023-03-14T05:11:55.805245+00:00\', \'SynchronizedTimeStamp\': \'2023-03-14T05:11:55.000000+00:00\', \'min_compatible_version\': \'3.0\', \'max_compatible_version\': \'\'}, Message: \n    [{\'AnalogInput_index0\': 0.1212,\n      \'AnalogInput_index1\': 1.2323,\n      \'AnalogInput_index2\': 0.0,\n      \'AnalogInput_index3\': 0.0,\n      \'AnalogOutput_index0\': 0.0,\n      \'AnalogOutput_index1\': 0.0,\n      \'AnalogOutput_index2\': 0.0,\n      \'AnalogOutput_index3\': 0.0,\n      \'BinaryInput_index0\': False,\n      \'BinaryInput_index1\': False,\n      \'BinaryInput_index2\': False,\n      \'BinaryInput_index3\': False,\n      \'BinaryOutput_index0\': False,\n      \'BinaryOutput_index1\': False,\n      \'BinaryOutput_index2\': False,\n      \'BinaryOutput_index3\': False},\n     {\'AnalogInput_index0\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogInput_index1\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogInput_index2\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogInput_index3\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogOutput_index0\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogOutput_index1\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogOutput_index2\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'AnalogOutput_index3\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryInput_index0\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryInput_index1\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryInput_index2\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryInput_index3\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryOutput_index0\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryOutput_index1\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryOutput_index2\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'},\n      \'BinaryOutput_index3\': {\'type\': \'integer\', \'tz\': \'UTC\', \'units\': \'NA\'}}]\n    2023-03-14 00:11:55,810 (volttron-platform-driver-0.2.0rc0 24737) volttron.driver.base.driver(334) DEBUG: finish publishing: devices/campus/building/dnp3/all\n    2023-03-14 00:11:56,825 (volttron-listener-0.2.0rc0 24424) listener.agent(104) INFO: Peer: pubsub, Sender: volttron-listener-0.2.0rc0_2:, Bus: , Topic: heartbeat/volttron-listener-0.2.0rc0_2, Headers: {\'TimeStamp\': \'2023-03-14T05:11:56.820827+00:00\', \'min_compatible_version\': \'3.0\', \'max_compatible_version\': \'\'}, Message: \n    \n    ```\n\n1. Shutdown the platform\n\n   ```shell\n   vctl shutdown --platform\n   ```\n\n# Development\n\nPlease see the following for contributing\nguidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide\nabout [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government. Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/eclipse-volttron/volttron-lib-dnp3-driver',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['volttron', 'volttron.driver.interfaces.dnp3']
 package_data = \ {'': ['*']} install_requires = \ ['dnp3-
 python>=0.2.3b2,<0.3.0', 'volttron-lib-base-driver>=0.2.0rc0,<0.3.0']
-setup_kwargs = { 'name': 'volttron-lib-dnp3-driver', 'version': '0.1.1a1',
+setup_kwargs = { 'name': 'volttron-lib-dnp3-driver', 'version': '0.1.1a2',
 'description': 'A minimal implementation of a driver for the VOLTTRON
 platform.', 'long_description': '# volttron-lib-dnp3-driver\n\n[//]: # (TODO:
 get the badges)\n\nDistributed Network Protocol (DNP\nor [DNP3](https://
 en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance since its
 introduction in 1993. This\nprotocol is an immediately deployable solution for
 monitoring remote sites because it was developed for communication of\ncritical
 infrastructure status, allowing for reliable remote control.\n\nDNP3 is
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a1/PKG-INFO` & `volttron_lib_dnp3_driver-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-dnp3-driver
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A minimal implementation of a driver for the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a1 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a2 Summary:
 A minimal implementation of a driver for the VOLTTRON platform. Home-page:
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver License: Apache-
 2.0 Author: VOLTTRON Team Author-email: volttron@pnnl.gov Requires-Python:
 >=3.8,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
```

