# Comparing `tmp/sdss_basecam-0.7.1b1.tar.gz` & `tmp/sdss_basecam-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_basecam-0.7.1b1.tar", max compression
+gzip compressed data, was "sdss_basecam-0.7.2.tar", max compression
```

## Comparing `sdss_basecam-0.7.1b1.tar` & `sdss_basecam-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1504 2019-06-19 23:49:42.000000 sdss_basecam-0.7.1b1/LICENSE.md
--rw-r--r--   0        0        0     1132 2021-02-13 08:53:15.106034 sdss_basecam-0.7.1b1/README.md
--rw-r--r--   0        0        0      290 2021-09-04 00:42:08.959313 sdss_basecam-0.7.1b1/basecam/__init__.py
--rw-r--r--   0        0        0      303 2020-01-14 20:12:52.000000 sdss_basecam-0.7.1b1/basecam/actor/__init__.py
--rw-r--r--   0        0        0     6097 2022-06-05 02:48:55.718704 sdss_basecam-0.7.1b1/basecam/actor/actor.py
--rw-r--r--   0        0        0      576 2021-02-16 20:08:20.779528 sdss_basecam-0.7.1b1/basecam/actor/commands/__doc_parser.py
--rw-r--r--   0        0        0      633 2021-02-16 20:05:43.026400 sdss_basecam-0.7.1b1/basecam/actor/commands/__init__.py
--rw-r--r--   0        0        0     2176 2021-05-16 23:35:00.962908 sdss_basecam-0.7.1b1/basecam/actor/commands/area.py
--rw-r--r--   0        0        0     1037 2023-03-10 07:34:48.796202 sdss_basecam-0.7.1b1/basecam/actor/commands/base.py
--rw-r--r--   0        0        0     1778 2021-05-16 23:35:13.070916 sdss_basecam-0.7.1b1/basecam/actor/commands/binning.py
--rw-r--r--   0        0        0     7980 2023-03-02 02:22:32.636161 sdss_basecam-0.7.1b1/basecam/actor/commands/expose.py
--rw-r--r--   0        0        0     2445 2021-02-15 04:41:55.937905 sdss_basecam-0.7.1b1/basecam/actor/commands/reconnect.py
--rw-r--r--   0        0        0     1382 2021-02-15 04:41:55.938105 sdss_basecam-0.7.1b1/basecam/actor/commands/set_default.py
--rw-r--r--   0        0        0     2060 2021-05-16 23:35:21.627547 sdss_basecam-0.7.1b1/basecam/actor/commands/shutter.py
--rw-r--r--   0        0        0     1004 2022-04-25 21:36:04.496020 sdss_basecam-0.7.1b1/basecam/actor/commands/status.py
--rw-r--r--   0        0        0     1973 2021-05-16 23:35:27.511693 sdss_basecam-0.7.1b1/basecam/actor/commands/temperature.py
--rw-r--r--   0        0        0     4435 2021-02-22 02:57:41.039223 sdss_basecam-0.7.1b1/basecam/actor/schema.json
--rw-r--r--   0        0        0     2605 2022-06-12 15:47:45.377567 sdss_basecam-0.7.1b1/basecam/actor/tools.py
--rw-r--r--   0        0        0    30223 2022-12-24 21:34:00.604916 sdss_basecam-0.7.1b1/basecam/camera.py
--rw-r--r--   0        0        0     1203 2021-02-22 02:57:41.040339 sdss_basecam-0.7.1b1/basecam/events.py
--rw-r--r--   0        0        0     2111 2021-02-08 23:56:50.499705 sdss_basecam-0.7.1b1/basecam/exceptions.py
--rw-r--r--   0        0        0    13080 2022-12-21 23:03:40.181473 sdss_basecam-0.7.1b1/basecam/exposure.py
--rw-r--r--   0        0        0     7505 2021-07-22 05:59:18.850781 sdss_basecam-0.7.1b1/basecam/mixins.py
--rw-r--r--   0        0        0       63 2021-02-10 20:56:49.521997 sdss_basecam-0.7.1b1/basecam/models/__init__.py
--rw-r--r--   0        0        0     1481 2021-09-04 00:42:08.968930 sdss_basecam-0.7.1b1/basecam/models/builtin.py
--rw-r--r--   0        0        0    17696 2021-09-04 00:42:08.973005 sdss_basecam-0.7.1b1/basecam/models/card.py
--rw-r--r--   0        0        0    10939 2022-06-05 22:22:40.459317 sdss_basecam-0.7.1b1/basecam/models/fits.py
--rw-r--r--   0        0        0     6716 2021-07-22 05:59:59.713417 sdss_basecam-0.7.1b1/basecam/notifier.py
--rw-r--r--   0        0        0     6132 2021-12-15 00:22:57.856498 sdss_basecam-0.7.1b1/basecam/utils.py
--rw-r--r--   0        0        0     2881 2023-03-10 07:45:37.336365 sdss_basecam-0.7.1b1/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 sdss_basecam-0.7.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-27 22:04:43.467543 sdss_basecam-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0     1132 2023-04-27 22:04:43.467974 sdss_basecam-0.7.2/README.md
+-rw-r--r--   0        0        0      290 2023-04-27 22:04:43.468393 sdss_basecam-0.7.2/basecam/__init__.py
+-rw-r--r--   0        0        0      303 2023-04-27 22:04:43.468808 sdss_basecam-0.7.2/basecam/actor/__init__.py
+-rw-r--r--   0        0        0     6096 2023-04-27 22:04:43.469155 sdss_basecam-0.7.2/basecam/actor/actor.py
+-rw-r--r--   0        0        0      576 2023-04-27 22:04:43.469547 sdss_basecam-0.7.2/basecam/actor/commands/__doc_parser.py
+-rw-r--r--   0        0        0      633 2023-04-27 22:04:43.469861 sdss_basecam-0.7.2/basecam/actor/commands/__init__.py
+-rw-r--r--   0        0        0     2175 2023-04-27 22:04:43.470179 sdss_basecam-0.7.2/basecam/actor/commands/area.py
+-rw-r--r--   0        0        0     1037 2023-04-27 22:04:43.470530 sdss_basecam-0.7.2/basecam/actor/commands/base.py
+-rw-r--r--   0        0        0     1777 2023-04-27 22:04:43.470840 sdss_basecam-0.7.2/basecam/actor/commands/binning.py
+-rw-r--r--   0        0        0     7980 2023-04-27 22:04:43.471183 sdss_basecam-0.7.2/basecam/actor/commands/expose.py
+-rw-r--r--   0        0        0     2444 2023-04-27 22:04:43.471502 sdss_basecam-0.7.2/basecam/actor/commands/reconnect.py
+-rw-r--r--   0        0        0     1382 2023-04-27 22:04:43.471816 sdss_basecam-0.7.2/basecam/actor/commands/set_default.py
+-rw-r--r--   0        0        0     2060 2023-04-27 22:04:43.472135 sdss_basecam-0.7.2/basecam/actor/commands/shutter.py
+-rw-r--r--   0        0        0     1004 2023-04-27 22:04:43.472445 sdss_basecam-0.7.2/basecam/actor/commands/status.py
+-rw-r--r--   0        0        0     1973 2023-04-27 22:04:43.472764 sdss_basecam-0.7.2/basecam/actor/commands/temperature.py
+-rw-r--r--   0        0        0     4435 2023-04-27 22:04:43.473240 sdss_basecam-0.7.2/basecam/actor/schema.json
+-rw-r--r--   0        0        0     2605 2023-04-27 22:04:43.473675 sdss_basecam-0.7.2/basecam/actor/tools.py
+-rw-r--r--   0        0        0    30342 2023-04-27 22:04:43.474255 sdss_basecam-0.7.2/basecam/camera.py
+-rw-r--r--   0        0        0     1203 2023-04-27 22:04:43.474673 sdss_basecam-0.7.2/basecam/events.py
+-rw-r--r--   0        0        0     2109 2023-04-27 22:04:43.475020 sdss_basecam-0.7.2/basecam/exceptions.py
+-rw-r--r--   0        0        0    13155 2023-04-27 22:04:43.475433 sdss_basecam-0.7.2/basecam/exposure.py
+-rw-r--r--   0        0        0     7505 2023-04-27 22:04:43.475816 sdss_basecam-0.7.2/basecam/mixins.py
+-rw-r--r--   0        0        0       63 2023-04-27 22:04:43.476231 sdss_basecam-0.7.2/basecam/models/__init__.py
+-rw-r--r--   0        0        0     1481 2023-04-27 22:04:43.476559 sdss_basecam-0.7.2/basecam/models/builtin.py
+-rw-r--r--   0        0        0    17690 2023-04-27 22:04:43.476983 sdss_basecam-0.7.2/basecam/models/card.py
+-rw-r--r--   0        0        0    10934 2023-04-27 22:04:43.477404 sdss_basecam-0.7.2/basecam/models/fits.py
+-rw-r--r--   0        0        0     6713 2023-04-27 22:04:43.477778 sdss_basecam-0.7.2/basecam/notifier.py
+-rw-r--r--   0        0        0     6130 2023-04-27 22:04:43.478179 sdss_basecam-0.7.2/basecam/utils.py
+-rw-r--r--   0        0        0     2876 2023-04-27 22:04:43.488875 sdss_basecam-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2317 1970-01-01 00:00:00.000000 sdss_basecam-0.7.2/PKG-INFO
```

### Comparing `sdss_basecam-0.7.1b1/LICENSE.md` & `sdss_basecam-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/README.md` & `sdss_basecam-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/actor.py` & `sdss_basecam-0.7.2/basecam/actor/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         camera_system: CameraSystem,
         *args,
         default_cameras: Union[List[str], str, None] = None,
         command_parser: clu.parsers.click.CluGroup | None = None,
         schema: Optional[str] = "internal",
         **kwargs,
     ):
-
         self._check_is_subclass()
 
         assert camera_system is not None
         self.camera_system = camera_system
 
         assert self.camera_system.camera_class
```

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/__doc_parser.py` & `sdss_basecam-0.7.2/basecam/actor/commands/__doc_parser.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/__init__.py` & `sdss_basecam-0.7.2/basecam/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/area.py` & `sdss_basecam-0.7.2/basecam/actor/commands/area.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
     cameras = get_cameras(command, cameras=cameras, fail_command=True)
     if not cameras:  # pragma: no cover
         return
 
     failed = False
     for camera in cameras:
-
         if not area and reset is False:
             report_area(command, camera, tuple(await camera.get_image_area()))
         else:
             if reset:
                 area = None
             try:
                 await camera.set_image_area(area)
```

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/base.py` & `sdss_basecam-0.7.2/basecam/actor/commands/base.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/binning.py` & `sdss_basecam-0.7.2/basecam/actor/commands/binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     cameras = get_cameras(command, cameras=cameras, fail_command=True)
     if not cameras:  # pragma: no cover
         return
 
     failed = False
     for camera in cameras:
-
         if not binning:
             binning = list(await camera.get_binning())
             command.info(
                 binning=dict(
                     camera=camera.name,
                     horizontal=binning[0],
                     vertical=binning[1],
```

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/expose.py` & `sdss_basecam-0.7.2/basecam/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/reconnect.py` & `sdss_basecam-0.7.2/basecam/actor/commands/reconnect.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
     cameras = get_cameras(command, cameras=cameras, fail_command=True)
     if not cameras:  # pragma: no cover
         return
 
     failed = False
     for camera in cameras:
-
         command.warning(text=f"reconnecting camera {camera.name!r}")
 
         try:
             await asyncio.wait_for(camera.disconnect(), timeout=timeout)
             command.info(
                 camera=camera.name, text=f"camera {camera.name!r} was disconnected."
             )
```

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/set_default.py` & `sdss_basecam-0.7.2/basecam/actor/commands/set_default.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/shutter.py` & `sdss_basecam-0.7.2/basecam/actor/commands/shutter.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/status.py` & `sdss_basecam-0.7.2/basecam/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/commands/temperature.py` & `sdss_basecam-0.7.2/basecam/actor/commands/temperature.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/schema.json` & `sdss_basecam-0.7.2/basecam/actor/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/actor/tools.py` & `sdss_basecam-0.7.2/basecam/actor/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/camera.py` & `sdss_basecam-0.7.2/basecam/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         include: Optional[List[Any]] = None,
         exclude: Optional[List[Any]] = None,
         logger: Optional[SDSSLogger] = None,
         log_header: Optional[str] = None,
         log_file: Optional[AnyPath] = None,
         verbose: Optional[Union[bool, int]] = False,
     ):
-
         self.camera_class = camera_class or self.camera_class
 
         if not self.camera_class or not issubclass(self.camera_class, BaseCamera):
             raise ValueError("camera_class must be a subclass of BaseCamera.")
 
         self.include = self.include or include
         self.exclude = self.exclude or exclude
@@ -407,15 +406,14 @@
             The name of the camera.
         uid
             The unique identifier for the camera.
         """
 
         for camera in self.cameras:
             if camera.name == name or camera.uid == uid:
-
                 await camera.disconnect()
                 self.cameras.remove(camera)
 
                 self.log(f"removed camera {camera.name!r}.")
 
                 # Notify event
                 self.notifier.notify(
@@ -567,15 +565,14 @@
         uid: str,
         camera_system: CameraSystem,
         name: Optional[str] = None,
         force: bool = False,
         image_namer: Optional[Union[ImageNamer, dict]] = None,
         camera_params={},
     ):
-
         self.uid = uid
         self.name = name or self.uid
 
         self.camera_system = camera_system
         self.loop = camera_system.loop
 
         self.connected = False
@@ -786,16 +783,15 @@
             "remaining_time": exptime,
             "image_type": image_type,
             "n_stack": stack,
             "current_stack": 1,
         }
 
         for idx in range(stack):
-
-            notif_payload.update({"n_stack": idx + 1})
+            notif_payload.update({"current_stack": idx + 1})
 
             exposure = Exposure(self, fits_model=fits_model)
             exposure.image_type = image_type
             exposure.exptime = exptime
 
             self.notify(CameraEvent.EXPOSURE_INTEGRATING, notif_payload)
             try:
@@ -808,15 +804,19 @@
                 error = "data was not taken."
                 self.notify(CameraEvent.EXPOSURE_FAILED, {"error": error})
                 raise ExposureError(error)
 
             exposures.append(exposure)
 
         if len(exposures) > 1:
-            data = [cast(numpy.ndarray, exp.data) for exp in exposures]
+            data = [
+                exp.data.astype(numpy.float32)
+                for exp in exposures
+                if exp.data is not None
+            ]
             stacked_data = stack_function(numpy.stack(data), axis=0)
             exposures[0].data = stacked_data
 
         exposure = exposures[0]
         exposure.exptime_n = exptime * stack
         exposure.stack = stack
         exposure.stack_function = stack_function
@@ -826,15 +826,16 @@
                 exposure.filename = str(filename)
         else:
             exposure.filename = str(filename or self.image_namer(self, num=num))
 
         notif_payload = {
             "exptime_total": exposure.exptime_n,
             "image_type": image_type,
-            "stack": stack,
+            "current_stack": 0,
+            "n_stack": 0,
         }
         self.notify(CameraEvent.EXPOSURE_DONE, notif_payload)
 
         if postprocess:
             try:
                 exposure = await self._post_process_internal(exposure, **kwargs)
             except ExposureError:
```

### Comparing `sdss_basecam-0.7.1b1/basecam/events.py` & `sdss_basecam-0.7.2/basecam/events.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/exceptions.py` & `sdss_basecam-0.7.2/basecam/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from . import camera
 
 
 class CameraError(Exception):
     """A custom core exception"""
 
     def __init__(self, message=""):
-
         stack = inspect.stack()
         f_locals = stack[1][0].f_locals
 
         if "self" in f_locals:
             class_ = f_locals["self"]
             if isinstance(class_, camera.BaseCamera):
                 camera_name = f_locals["self"].name
@@ -48,15 +47,14 @@
     """Error raised by a FITS `.Card`."""
 
 
 class CameraWarning(UserWarning):
     """Base warning."""
 
     def __init__(self, message, *args, **kwargs):
-
         stack = inspect.stack()
         f_locals = stack[1][0].f_locals
 
         if "self" in f_locals:
             class_ = f_locals["self"]
             if isinstance(class_, camera.BaseCamera):
                 camera_name = f_locals["self"].name
```

### Comparing `sdss_basecam-0.7.1b1/basecam/exposure.py` & `sdss_basecam-0.7.2/basecam/exposure.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         self,
         camera: basecam.camera.BaseCamera,
         filename: Optional[str] = None,
         data: Optional[numpy.ndarray] = None,
         fits_model: Optional[basecam.models.FITSModel] = None,
         wcs: Optional[astropy.wcs.WCS] = None,
     ):
-
         self.camera = camera
         self.data = data
         self.fits_model = fits_model.copy() if fits_model else None
         self.filename = filename
 
         self._obstime: astropy.time.Time = astropy.time.Time.now()
 
@@ -113,15 +112,14 @@
         format; in the latter case, UTC scale is assumed.
         """
 
         return self._obstime
 
     @obstime.setter
     def obstime(self, value: astropy.time.Time):
-
         if isinstance(value, astropy.time.Time):
             self._obstime = value
         elif isinstance(value, str):
             self._obstime = astropy.time.Time(value, format="iso", scale="utc")
         else:
             raise ExposureError(f"invalid obstime {value}")
 
@@ -217,15 +215,14 @@
         loop = asyncio.get_event_loop()
 
         filename = str(filename)
 
         for ntry in range(2):
             try:
                 if filename.endswith(".gz"):
-
                     # We compress in a local temporary file, which is faster when we are
                     # going to save a file across the network.
                     tmp_name = tempfile.NamedTemporaryFile(suffix=".gz").name
 
                     # Astropy compresses with gzip -9 which takes forever.
                     # Instead we compress manually with -1, which is still pretty good.
                     writeto_partial = functools.partial(
@@ -236,15 +233,14 @@
                     )
                     await loop.run_in_executor(None, writeto_partial)
                     await gzip_async(tmp_name[:-3], complevel=1)
 
                     shutil.move(tmp_name, filename)
 
                 else:
-
                     writeto_partial = functools.partial(
                         hdulist.writeto,
                         filename,
                         overwrite=overwrite,
                         checksum=checksum,
                     )
 
@@ -261,19 +257,21 @@
                 else:
                     raise ExposureError(f"Failed writing exposure to disk: {err}")
 
         # Horrible hack to try to fix compressed headers.
         update_hdu = fits.open(filename, mode="update")
         for ext in update_hdu:
             try:
-                BSCALE = ext.header.pop("BSCALE", 1)
-                BZERO = ext.header.pop("BZERO", 2**15)
-                ext.header["BSCALE"] = BSCALE
-                ext.header["BZERO"] = BZERO
+                if "BSCALE" in ext.header:
+                    BSCALE = ext.header.pop("BSCALE", 1)
+                    BZERO = ext.header.pop("BZERO", 2**15)
+                    ext.header["BSCALE"] = BSCALE
+                    ext.header["BZERO"] = BZERO
             except Exception:
+                raise
                 pass
         update_hdu.close()
 
         return hdulist
 
 
 class ImageNamer(object):
@@ -315,15 +313,14 @@
         self,
         basename: str = "{camera.name}-{num:04d}.fits",
         dirname: str = ".",
         overwrite: bool = False,
         camera: Optional[basecam.camera.BaseCamera] = None,
         reset_sequence: bool = True,
     ):
-
         assert re.match(r".+(\{num.+\}).+", basename), "invalid basename."
 
         self._basename: str
         self.basename = basename
 
         self.dirname: Union[pathlib.Path, str] = pathlib.Path(dirname)
         self.overwrite: bool = overwrite
@@ -390,15 +387,14 @@
 
     def __call__(
         self,
         camera: Optional[basecam.camera.BaseCamera] = None,
         update_num: bool = True,
         num: Optional[int] = None,
     ) -> pathlib.Path:
-
         camera = camera or self.camera
 
         if camera:
             expanded_basename = self.basename.format(camera=camera)
         else:
             expanded_basename = self.basename.format()
```

### Comparing `sdss_basecam-0.7.1b1/basecam/mixins.py` & `sdss_basecam-0.7.2/basecam/mixins.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/models/builtin.py` & `sdss_basecam-0.7.2/basecam/models/builtin.py`

 * *Files identical despite different names*

### Comparing `sdss_basecam-0.7.1b1/basecam/models/card.py` & `sdss_basecam-0.7.2/basecam/models/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
     context
         A dictionary of parameters used to fill the value replacement fields.
         Two values, ``__exposure__`` and ``__camera__``, are always defined.
         This context can be updated during the evaluation of the card.
     """
 
     def __new__(cls, name: Union[str, Iterable[Any]], *args, **kwargs):
-
         if isinstance(name, str):
             if cls == Card and name.upper() in DEFAULT_CARDS:
                 if len(args) == 0 and len(kwargs) == 0:
                     return DEFAULT_CARDS[name.upper()]
             return super().__new__(cls)
 
         return cls(*name)
@@ -124,15 +123,14 @@
         type: Optional[type] = None,
         autocast: bool = True,
         default: Any = None,
         fargs: Optional[tuple] = None,
         evaluate: bool = False,
         context: Dict[str, Any] = {},
     ):
-
         if hasattr(self, "name"):
             return
 
         assert isinstance(name, str)
 
         self.name = name
         if len(self.name) > 8:
@@ -293,23 +291,21 @@
 
     def __init__(
         self,
         cards: Iterable[Union[Card, Iterable, str]],
         name: Optional[str] = None,
         use_group_title: bool = True,
     ):
-
         self.name = name or self.name
         self.use_group_title: bool = use_group_title
 
         cards = [self._process_input(card) for card in cards or []]
         list.__init__(self, cards)
 
     def __repr__(self):
-
         return f"<CardGroup {list.__repr__(self)!s}>"
 
     def _process_input(self, card: Union[Card, Iterable]):
         """Processes the input and converts it into a valid card."""
 
         if isinstance(card, Card):
             return card
@@ -398,21 +394,19 @@
 
     def __init__(
         self,
         name: Optional[str] = None,
         use_group_title: bool = False,
         **kwargs,
     ):
-
         self.name = name or self.name
         self.use_group_title = use_group_title
         self.kwargs = kwargs
 
     def __repr__(self):
-
         return f"<{self.__class__.__name__} (name={self.name})>"
 
     @abc.abstractmethod
     def macro(self, exposure: Exposure, context: Dict[str, Any] = {}):
         """The macro.
 
         Must return a list of item which can be tuples with the format
```

### Comparing `sdss_basecam-0.7.1b1/basecam/models/fits.py` & `sdss_basecam-0.7.2/basecam/models/fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     """
 
     def __init__(
         self,
         extensions: Optional[List[Extension]] = None,
         context: Dict[str, Any] = {},
     ):
-
         self.context: Dict[str, Any] = context
 
         extensions = extensions or []
         list.__init__(self, extensions)
 
         if len(self) == 0:
             self.append(Extension(data="raw", name="DATA"))
@@ -151,15 +150,14 @@
         self,
         data: Union[Literal["raw"], Literal["none"], None, bool, numpy.ndarray] = None,
         header_model: Optional[HeaderModel] = None,
         name: Optional[str] = None,
         compressed: Union[bool, str] = False,
         compression_params: dict[str, Any] = {},
     ):
-
         if isinstance(data, numpy.ndarray):
             self.data = data
         else:
             assert data is None or data in self.__VALID_DATA_VALUES, "invalid data"
             self.data = data
 
         self.header_model = header_model
@@ -267,20 +265,18 @@
     >>> header_model = HeaderModel([Card('TELESCOP', 'APO-2.5', 'The telescope'),
                                     Card('OBSERVATORY', 'APO'),
                                     'EXPTIME',
                                     Card('camname', '{(camera).name}')])
     """
 
     def __init__(self, cards: List[_CardTypes] = []):
-
         cards = [self._process_input(card) for card in cards]
         list.__init__(self, cards)
 
     def __repr__(self):
-
         return f"<HeaderModel {list.__repr__(self)!s}>"
 
     def _process_input(self, input_card: _CardTypes) -> _CardTypes:
         """Processes the input and converts it into a valid card."""
 
         if isinstance(input_card, (Card, CardGroup, MacroCard)):
             return input_card
@@ -323,15 +319,14 @@
             A `~astropy.io.fits.Header`, created by evaluating the model for
             the input exposure.
         """
 
         header = astropy.io.fits.Header()
 
         for card in self:
-
             processed_card = self._process_input(card)
             if processed_card is not None:
                 if isinstance(processed_card, Card):
                     header.append(processed_card.evaluate(exposure, context=context))
                 elif isinstance(processed_card, (CardGroup, MacroCard)):
                     header += processed_card.to_header(exposure, context=context)
```

### Comparing `sdss_basecam-0.7.1b1/basecam/notifier.py` & `sdss_basecam-0.7.2/basecam/notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     """A registry of clients to be notified of events.
 
     Allows to register a listener queue in which to announce events.
 
     """
 
     def __init__(self):
-
         self.listeners = []
 
     def register_listener(self, listener):
         """Registers a listener.
 
         Parameters
         ----------
@@ -60,15 +59,14 @@
             A dictionary with the information associated with the event.
 
         """
 
         assert isinstance(event, enum.Enum), "event is not an enum."
 
         for listener in self.listeners:
-
             if listener.filter_events and event not in listener.filter_events:
                 return False
 
             listener.put_nowait((event, payload))
 
         return True
 
@@ -83,15 +81,14 @@
         all events will be notified.
     autostart : bool
         Whether to start the listener as soon as the object is created.
 
     """
 
     def __init__(self, loop=None, filter_events=None, autostart=True):
-
         asyncio.Queue.__init__(self)
 
         self.callbacks = []
 
         self.loop = loop or asyncio.get_running_loop()
 
         self.filter_events = filter_events
```

### Comparing `sdss_basecam-0.7.1b1/basecam/utils.py` & `sdss_basecam-0.7.2/basecam/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         Initial delay between calls to the callback.
     loop : event loop
         The event loop to which to attach the task.
 
     """
 
     def __init__(self, name, callback, delay=1, loop=None):
-
         self.name = name
         self.callback = callback
 
         self._orig_delay = delay
         self.delay = delay
 
         self.loop = loop or asyncio.get_event_loop()
@@ -67,15 +66,14 @@
         self._sleep_task = None
         self._task = None
 
     async def poller(self):
         """The polling loop."""
 
         while True:
-
             try:
                 if asyncio.iscoroutinefunction(self.callback):
                     await self.callback()
                 else:
                     self.callback()
             except Exception as ee:
                 self.loop.call_exception_handler(
```

### Comparing `sdss_basecam-0.7.1b1/pyproject.toml` & `sdss_basecam-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-basecam"
-version = "0.7.1b1"
+version = "0.7.2"
 description = "A base library for camera wrapping and actor."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD 3-Clause License"
 readme = "README.md"
 homepage = "https://github.com/sdss/basecam"
 repository = "https://github.com/sdss/basecam"
 documentation = "https://sdss-basecam.readthedocs.io/en/latest/"
@@ -21,15 +21,15 @@
     { include = "basecam" }
 ]
 include = ["basecam/actor/schema.json"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<4.0"
 astropy = "^5.2"
-sdss-clu = ">=2.0.0b2"
+sdss-clu = "^2.0.0"
 sdsstools = ">=0.5.2"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 matplotlib = ">=3.1.1"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
```

### Comparing `sdss_basecam-0.7.1b1/PKG-INFO` & `sdss_basecam-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-basecam
-Version: 0.7.1b1
+Version: 0.7.2
 Summary: A base library for camera wrapping and actor.
 Home-page: https://github.com/sdss/basecam
 License: BSD 3-Clause License
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.2,<6.0)
-Requires-Dist: sdss-clu (>=2.0.0b2)
+Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
 Requires-Dist: sdsstools (>=0.5.2)
 Project-URL: Documentation, https://sdss-basecam.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/basecam
 Description-Content-Type: text/markdown
 
 basecam
 =======
```

