# Comparing `tmp/astro-drpy-0.0.1.6.tar.gz` & `tmp/astro-drpy-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-drpy-0.0.1.6.tar", last modified: Thu Apr 13 06:39:09 2023, max compression
+gzip compressed data, was "astro-drpy-0.0.1.7.tar", last modified: Fri Apr 28 04:51:55 2023, max compression
```

## Comparing `astro-drpy-0.0.1.6.tar` & `astro-drpy-0.0.1.7.tar`

### file list

```diff
@@ -1,535 +1,540 @@
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/LICENSE
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2023-02-06 04:59:52.000000 astro-drpy-0.0.1.6/README.md
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1082 2023-02-08 17:46:37.000000 astro-drpy-0.0.1.6/pyproject.toml
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      106 2023-04-04 16:27:59.000000 astro-drpy-0.0.1.6/requirements.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/setup.cfg
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2022-12-01 18:47:37.000000 astro-drpy-0.0.1.6/setup.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.772295 astro-drpy-0.0.1.6/src/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.796296 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    25421 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/SOURCES.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/dependency_links.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      107 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/requires.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/top_level.txt
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.804296 astro-drpy-0.0.1.6/src/drpy/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1080 2023-04-10 12:06:57.000000 astro-drpy-0.0.1.6/src/drpy/__init__.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.812296 astro-drpy-0.0.1.6/src/drpy/batch/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      108 2023-02-05 14:09:14.000000 astro-drpy-0.0.1.6/src/drpy/batch/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    18108 2023-04-09 09:14:51.000000 astro-drpy-0.0.1.6/src/drpy/batch/core.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.840297 astro-drpy-0.0.1.6/src/drpy/image/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      109 2023-02-05 14:09:48.000000 astro-drpy-0.0.1.6/src/drpy/image/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2624 2023-04-08 16:02:07.000000 astro-drpy-0.0.1.6/src/drpy/image/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     9178 2023-04-10 16:29:40.000000 astro-drpy-0.0.1.6/src/drpy/image/utils.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.868298 astro-drpy-0.0.1.6/src/drpy/modeling/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      175 2023-02-05 14:11:42.000000 astro-drpy-0.0.1.6/src/drpy/modeling/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    16057 2023-04-10 05:38:40.000000 astro-drpy-0.0.1.6/src/drpy/modeling/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1165 2022-11-29 12:56:55.000000 astro-drpy-0.0.1.6/src/drpy/modeling/function.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.884298 astro-drpy-0.0.1.6/src/drpy/onedspec/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      380 2023-02-05 14:12:22.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8887 2023-02-05 14:12:32.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/center.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    24324 2023-04-10 14:57:51.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8555 2023-02-08 17:48:04.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/io.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.772295 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.888298 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/extinction/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      191 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/extinction/baoextinct.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.908299 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    13707 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/README
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.004302 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1918 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/h.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/i.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/j.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/k.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5237 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/l.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5242 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3762 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      602 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      598 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8770 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/params.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/r.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      224 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/u.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/v.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.116306 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr3454.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr3982.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr4468.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr4534.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr5511.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      479 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7596.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7950.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr8634.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr9087.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.232310 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi1m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      680 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      168 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4mech.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14757 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14745 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    15440 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4484 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5212 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4501 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      607 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.572321 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      466 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/bd25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      465 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/bd8.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      706 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      652 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/h600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      543 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      544 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/kopf27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      673 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      551 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      662 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      595 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      648 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      693 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      580 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      906 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      592 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      717 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      870 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      497 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds749.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      387 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      719 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      932 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      194 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      995 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      445 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctioextinct.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.064337 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2028 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1209 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2078 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1299 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2011 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1302 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1182 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2065 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1127 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2059 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1229 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2046 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1213 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2018 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2123 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1292 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1156 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2012 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2080 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1245 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2038 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1207 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2032 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1197 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2093 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2014 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1181 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.236343 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1167 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244272 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   249264 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   125712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244992 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244368 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248640 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   249120 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248784 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   104112 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   126960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244944 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   114000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   102480 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   125472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   104016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   123696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246912 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   106869 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   109053 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54999 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107184 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   106911 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108990 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    45549 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    55545 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107163 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    49875 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    44835 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54894 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    45507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54117 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107625 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108024 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108045 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.272344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/40erib.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd253941.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd332642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd404032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd82015.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige24.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige92.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g4718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      499 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/gd190.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw705824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw708247.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      455 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw738031.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hiltner102.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      414 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz29.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      427 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz43.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      431 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz7.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/kopff27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l13633.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l151234b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l74546a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      432 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l8702.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      433 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lb1240.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lds235b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      839 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ross640.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/sa29130.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1336 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      434 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ton573.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      450 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/wolf485a.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.284344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1193 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1239 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1253 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1252 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1172 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1173 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1162 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1257 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1176 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1232 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1255 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1271 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1294 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      137 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      523 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1062 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      950 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/names.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.288344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1105 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1083 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1132 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1134 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      111 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      188 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.436349 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      681 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.444349 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      685 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1454 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1393 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      756 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1574 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      728 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      724 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      811 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      682 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      782 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      713 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      763 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1373 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1376 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1557 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      612 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      773 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1577 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      776 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      768 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      738 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      606 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      631 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      775 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      774 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1807 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.456350 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6283 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3916 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6180 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3844 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6234 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3747 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3886 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6259 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6238 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      677 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      988 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.464350 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2531 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2536 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2530 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      152 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2535 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2220 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      627 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.488351 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      661 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      138 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      617 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      641 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      416 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    10234 2023-04-13 06:32:54.000000 astro-drpy-0.0.1.6/src/drpy/plotting.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.496351 astro-drpy-0.0.1.6/src/drpy/twodspec/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      353 2023-02-05 14:13:11.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    70816 2023-04-13 06:36:02.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/longslit.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3268 2023-02-21 15:22:01.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/utils.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1704 2022-11-30 07:57:09.000000 astro-drpy-0.0.1.6/src/drpy/utils.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    13466 2023-04-11 14:42:08.000000 astro-drpy-0.0.1.6/src/drpy/validate.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.698669 astro-drpy-0.0.1.7/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/LICENSE
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-28 04:51:55.698669 astro-drpy-0.0.1.7/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2023-02-06 04:59:52.000000 astro-drpy-0.0.1.7/README.md
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1082 2023-02-08 17:46:37.000000 astro-drpy-0.0.1.7/pyproject.toml
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      106 2023-04-04 16:27:59.000000 astro-drpy-0.0.1.7/requirements.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-28 04:51:55.698669 astro-drpy-0.0.1.7/setup.cfg
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2022-12-01 18:47:37.000000 astro-drpy-0.0.1.7/setup.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.914643 astro-drpy-0.0.1.7/src/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.922644 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-28 04:51:54.000000 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    25547 2023-04-28 04:51:54.000000 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-28 04:51:54.000000 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      107 2023-04-28 04:51:54.000000 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/requires.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-28 04:51:54.000000 astro-drpy-0.0.1.7/src/astro_drpy.egg-info/top_level.txt
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.942644 astro-drpy-0.0.1.7/src/drpy/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1080 2023-04-13 07:33:45.000000 astro-drpy-0.0.1.7/src/drpy/__init__.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.958645 astro-drpy-0.0.1.7/src/drpy/batch/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      108 2023-02-05 14:09:14.000000 astro-drpy-0.0.1.7/src/drpy/batch/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    18108 2023-04-09 09:14:51.000000 astro-drpy-0.0.1.7/src/drpy/batch/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       12 2023-04-24 07:18:28.000000 astro-drpy-0.0.1.7/src/drpy/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      361 2023-04-21 07:30:26.000000 astro-drpy-0.0.1.7/src/drpy/decorate.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.982646 astro-drpy-0.0.1.7/src/drpy/image/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      109 2023-02-05 14:09:48.000000 astro-drpy-0.0.1.7/src/drpy/image/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2595 2023-04-21 04:17:22.000000 astro-drpy-0.0.1.7/src/drpy/image/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    10432 2023-04-14 16:43:02.000000 astro-drpy-0.0.1.7/src/drpy/image/utils.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.998646 astro-drpy-0.0.1.7/src/drpy/modeling/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      175 2023-02-05 14:11:42.000000 astro-drpy-0.0.1.7/src/drpy/modeling/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    16842 2023-04-22 06:50:56.000000 astro-drpy-0.0.1.7/src/drpy/modeling/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1165 2022-11-29 12:56:55.000000 astro-drpy-0.0.1.7/src/drpy/modeling/function.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.014647 astro-drpy-0.0.1.7/src/drpy/onedspec/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      380 2023-02-05 14:12:22.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8911 2023-04-23 14:12:28.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/center.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    35997 2023-04-24 06:51:21.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8428 2023-04-23 12:06:25.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/io.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:54.914643 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.018647 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/extinction/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      191 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/extinction/baoextinct.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.042648 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    13707 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/README
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.066648 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1918 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/h.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/i.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/j.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/k.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5237 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/l.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5242 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3762 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      602 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      598 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8770 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/params.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/r.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      224 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/u.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/v.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.078649 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr3454.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr3982.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr4468.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr4534.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr5511.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      479 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr7596.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr7950.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr8634.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/hr9087.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/bstdscal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.158651 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/multi1m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      680 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      168 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/multi4mech.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14757 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14745 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    15440 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4484 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5212 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4501 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      607 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.198653 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      466 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/bd25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      465 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/bd8.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      706 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/f110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/f15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/f25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/f56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/f98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      652 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/h600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/hz15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      543 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      544 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/kopf27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      673 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      551 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      662 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      595 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      648 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      693 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      580 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      906 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      592 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      717 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      870 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      497 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/lds749.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      387 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      719 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      932 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      194 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/w1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      995 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      445 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctioextinct.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.234654 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2028 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1209 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2078 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1299 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2011 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1302 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1182 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2065 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1127 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2059 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1229 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2046 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1213 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2018 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2123 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1292 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1156 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2012 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2080 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1245 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2038 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1207 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2032 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1197 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2093 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2014 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1181 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.334657 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1167 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244272 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   249264 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   125712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244992 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244368 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248640 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   249120 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248784 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   104112 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   126960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244944 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   114000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   102480 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   125472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   104016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   123696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246912 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   106869 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   109053 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54999 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107184 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   106911 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108990 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    45549 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    55545 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107163 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    49875 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    44835 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54894 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    45507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54117 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107625 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108024 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108045 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.354658 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/40erib.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/bd253941.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/bd332642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/bd404032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/bd82015.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige24.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige92.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/feige98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/g4718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      499 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/gd190.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/grw705824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/grw708247.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      455 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/grw738031.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hiltner102.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      414 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz29.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      427 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz43.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      431 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/hz7.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/kopff27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l13633.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l151234b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l74546a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      432 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l8702.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      433 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/lb1240.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/lb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/lds235b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/lds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      839 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/ross640.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/sa29130.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1336 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      434 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/ton573.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      450 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/wolf485a.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.362658 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1193 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1239 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1253 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1252 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1172 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1173 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1162 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1257 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1176 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1232 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1255 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1271 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1294 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      137 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      523 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1062 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      950 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/names.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.366658 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1105 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1083 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1132 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1134 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      111 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      188 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.614667 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      681 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.626667 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      685 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1454 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1393 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      756 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1574 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      728 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      724 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      811 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      682 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      782 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      713 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      763 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1373 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1376 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1557 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      612 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      773 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1577 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      776 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      768 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      738 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      606 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      631 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      775 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      774 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1807 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.634667 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6283 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3916 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6180 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3844 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6234 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3747 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3886 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6259 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6238 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      677 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      988 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.642667 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2531 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2536 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2530 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      152 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2535 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2220 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      627 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.650668 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      661 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      138 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      617 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      641 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      416 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    10312 2023-04-23 16:41:49.000000 astro-drpy-0.0.1.7/src/drpy/plotting.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-28 04:51:55.686669 astro-drpy-0.0.1.7/src/drpy/twodspec/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      373 2023-04-22 07:28:36.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       64 2023-04-24 05:44:40.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/background.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       63 2023-04-24 05:44:22.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/extract.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    81815 2023-04-24 06:37:28.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/longslit.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      244 2023-04-24 07:03:13.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/trace.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3268 2023-02-21 15:22:01.000000 astro-drpy-0.0.1.7/src/drpy/twodspec/utils.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1704 2023-04-23 11:48:39.000000 astro-drpy-0.0.1.7/src/drpy/utils.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    13815 2023-04-22 16:08:59.000000 astro-drpy-0.0.1.7/src/drpy/validate.py
```

### Comparing `astro-drpy-0.0.1.6/LICENSE` & `astro-drpy-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/PKG-INFO` & `astro-drpy-0.0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-drpy
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: A data reduction toolkit for astronomical photometry and spectroscopy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/drpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/drpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-drpy-0.0.1.6/README.md` & `astro-drpy-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/pyproject.toml` & `astro-drpy-0.0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/astro_drpy.egg-info/PKG-INFO` & `astro-drpy-0.0.1.7/src/astro_drpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-drpy
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: A data reduction toolkit for astronomical photometry and spectroscopy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/drpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/drpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-drpy-0.0.1.6/src/astro_drpy.egg-info/SOURCES.txt` & `astro-drpy-0.0.1.7/src/astro_drpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup.py
 src/astro_drpy.egg-info/PKG-INFO
 src/astro_drpy.egg-info/SOURCES.txt
 src/astro_drpy.egg-info/dependency_links.txt
 src/astro_drpy.egg-info/requires.txt
 src/astro_drpy.egg-info/top_level.txt
 src/drpy/__init__.py
+src/drpy/core.py
+src/drpy/decorate.py
 src/drpy/plotting.py
 src/drpy/utils.py
 src/drpy/validate.py
 src/drpy/batch/__init__.py
 src/drpy/batch/core.py
 src/drpy/image/__init__.py
 src/drpy/image/core.py
@@ -499,9 +501,12 @@
 src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat
 src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat
 src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat
 src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat
 src/drpy/onedspec/lib/onedstds/spechayescal/standards.men
 src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat
 src/drpy/twodspec/__init__.py
+src/drpy/twodspec/background.py
+src/drpy/twodspec/extract.py
 src/drpy/twodspec/longslit.py
+src/drpy/twodspec/trace.py
 src/drpy/twodspec/utils.py
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/__init__.py` & `astro-drpy-0.0.1.7/src/drpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 # AstroPy
 from astropy import config as _config
 
 __all__ = ['__version__', 'conf']
 
-__version__ = '0.0.1.6'
+__version__ = '0.0.1.7'
 
 
 class Conf(_config.ConfigNamespace):
     """Configuration parameters for `drpy`."""
 
     # Unit
     unit_ccddata = _config.ConfigItem(
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/batch/core.py` & `astro-drpy-0.0.1.7/src/drpy/batch/core.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/image/core.py` & `astro-drpy-0.0.1.7/src/drpy/image/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-from copy import deepcopy
 
 # AstroPy
 from astropy.time import Time
 # ccdproc
 from ccdproc.utils.slices import slice_from_string
 # drpy
 from drpy.validate import _validate1DArray, _validateCCDList
@@ -63,15 +62,15 @@
         uncertainty_arr[python_slice] = (
             ccdlist[0].uncertainty.array[python_slice] * scale[0])
 
     if (ccdlist[0].mask is None) | (ccdlist[1].mask is None):
         mask_arr = None
 
     else:
-        mask_arr = deepcopy(ccdlist[1].mask)
+        mask_arr = ccdlist[1].mask.copy()
         mask_arr[python_slice] = ccdlist[0].mask[python_slice]
 
     nccd = ccdlist[0].copy()
 
     nccd.data = data_arr
 
     if uncertainty_arr is None:
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/image/utils.py` & `astro-drpy-0.0.1.7/src/drpy/image/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 # NumPy
 import numpy as np
 # SciPy
 from scipy.optimize import curve_fit, OptimizeWarning
 # matplotlib
 import matplotlib.pyplot as plt
+from matplotlib.backends.backend_pdf import PdfPages
 # AstroPy
 from astropy.nddata import Cutout2D
-from astropy.stats import gaussian_sigma_to_fwhm
+from astropy.stats import gaussian_sigma_to_fwhm, sigma_clip
 # photutils
 from photutils import CircularAperture, RectangularAperture
 from photutils.background import Background2D
 from photutils.centroids import centroid_com
 from photutils.detection import find_peaks
 # drpy
 from drpy import conf
@@ -25,18 +26,18 @@
 plt.rcParams['figure.figsize'] = [conf.fig_width, conf.fig_width]
 plt.rcParams['axes.linewidth'] = 1.5
 plt.rcParams['mathtext.fontset'] = 'stix'
 plt.rcParams['font.family'] = 'STIXGeneral'
 
 __all__ = ['getFWHM']
 
-# todo: deal with NaNs in Gaussian fitting.
-def getFWHM(ccd, box_size, n_sigma, aper_radius, saturation, n_peak, use_mask=False, 
-            title='FWHM', show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, 
-            **kwargs):
+
+def getFWHM(ccd, box_size, n_sigma, aper_radius, saturation, n_peak, n_iter=5, 
+            sigma_lower=None, sigma_upper=None, use_mask=False, title='fwhm', 
+            show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, **kwargs):
     """Estimate mean FWHM of the sources in the input image.
 
     The background of the input image is first modeled by a 2-dimensional background 
     estimator, and then subtracted from the input image. Detect sources in the 
     background subtracted image. Fit circular Gaussian profiles to the detected 
     sources.
 
@@ -61,14 +62,26 @@
     saturation : scalar
         Saturation level of pixels.
 
     n_peak : int
         Number of peaks. When number of peaks exceeds ``n_peak``, the peaks with the 
         highest peak intensities are used in determining FWHM.
 
+    n_iter : int, optional
+        Number of sigma slipping iterations. Must be >= `0`.
+        Default is `5`.
+
+    sigma_lower : scalar or `None`, optional
+        Number of standard deviations to use as the lower bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    sigma_upper : scalar or `None`, optional
+        Number of standard deviations to use as the upper bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
     use_mask : bool, optional
         If `True` and a mask array is attributed to ``ccd``, the masked pixels are 
         ignored in the background estimation and source detection. 
         Default is `False`.
 
     Returns
     -------
@@ -165,102 +178,120 @@
                 popt, _ = curve_fit(
                     CircularGaussian, xy, cutout2d_arr[i].flatten(), p0=initial_guess)
 
                 a, x0, y0, sigma, b = popt
 
                 if (a > 0) & (xy_min < x0 < xy_max) & (xy_min < y0 < xy_max):
                     position_arr[i] = x0 + size // 2, y0 + size // 2
-                    fwhm_arr[i] = sigma * gaussian_sigma_to_fwhm
+                    fwhm_arr[i] = np.abs(sigma) * gaussian_sigma_to_fwhm
                     cutout2d_arr[i] -= b
 
                 else:
                     raise RuntimeError('No feature fitted in the given region.')
 
             except (RuntimeError, TypeError, OptimizeWarning): # raise exception here
                 pass
 
     # Output
-    fwhm, fwhm_err = np.nanmean(fwhm_arr), np.nanstd(fwhm_arr, ddof=1)
+    fwhm_arr_masked, threshold_lower, threshold_upper = sigma_clip(
+        data=fwhm_arr, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+        maxiters=n_iter, stdfunc='mad_std', masked=True, return_bounds=True)
+    fwhm, fwhm_err = fwhm_arr_masked.mean(), fwhm_arr_masked.std(ddof=1)
+
+    if fwhm_arr_masked.mask.sum() > 0:
+        warnings.warn(
+            'Fitting for some sources failed (may caused by cosmic rays).', 
+            RuntimeWarning
+        )
 
     # Plot
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-    if title != 'FWHM':
-        title = [f'{title} FWHM (source detection)', 
-                 f'{title} FWHM (Gaussian2D fitting)']
-    else:
-        title = [f'FWHM (source detection)', f'FWHM (Gaussian2D fitting)']
-
-    fig_path = _validatePath(save, path, title)
+    _validateBool(save, 'save')
 
     if show | save:
 
-        # Source detection
+        _validateString(title, 'title')
+        if title != 'fwhm':
+            title = [f'{title} fwhm (source detection)', 
+                     f'{title} fwhm (cutoff)']
+        else:
+            title = [f'fwhm (source detection)', f'fwhm (cutoff)']
+
+        # Source detection plot
         fig, ax = plt.subplots(1, 1, dpi=100)
+
         # Image
-        extent = (
-            0.5, data_arr_bkgsb.shape[1] + 0.5, 0.5, data_arr_bkgsb.shape[0] + 0.5
-        )
-        _plot2d(ax=ax, ccd=data_arr_bkgsb, cmap='Greys_r', extent=extent)
+        _plot2d(ax=ax, ccd=data_arr_bkgsb, cmap='Greys_r')
         (xmin, xmax), (ymin, ymax) = ax.get_xlim(), ax.get_ylim()
         # Mask
         ax.imshow(
-            mask_arr, cmap='Greys', alpha=0.3 * mask_arr.astype(int), origin='lower', 
-            extent=extent)
+            mask_arr, cmap='Greys', alpha=0.3 * mask_arr.astype(int), origin='lower')
         # Aperture
         apertures = RectangularAperture(
-            positions=np.transpose([x + 1, y + 1]), w=size, h=size, theta=0)
-        apertures.plot(ax, color='r', lw=1)
+            positions=np.transpose([x, y]), w=size, h=size, theta=0)
+        apertures[fwhm_arr_masked.mask].plot(ax, color='b', lw=1)
+        apertures[~fwhm_arr_masked.mask].plot(ax, color='r', lw=1)
+
         # Setting
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
+        ax.annotate(
+            'masked', xy=(0.75, 0.88), xycoords='axes fraction', fontsize=16, 
+            color='b')
+        ax.annotate(
+            'detected', xy=(0.75, 0.93), xycoords='axes fraction', fontsize=16, 
+            color='r')
         ax.set_title(title[0], fontsize=16)
         fig.set_figheight(
             (data_arr_bkgsb.shape[0] / data_arr_bkgsb.shape[1] * fig.get_figwidth()))
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path[0], dpi=100)
+        if save:
+            fig_path = _validatePath(path, title[0])
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
-        # Cutout
-        if (n_peak % 4) == 0:
-            nrow = n_peak // 4
-        else:
-            nrow = n_peak // 4 + 1
-        extent = (0.5, size + 0.5, 0.5, size + 0.5)
+    # Cutout
+    if save:
 
-        fig = plt.figure(figsize=(10, 2 * nrow), dpi=100)
-        for i in range(n_peak):
-            ax = fig.add_subplot(nrow, 4, i + 1)
-            # Image
-            _plot2d(
-                ax=ax, ccd=cutout2d_arr[i], cmap='Greys_r', extent=extent, cbar=False, 
-                xlabel=None, ylabel=None)
-            # Aperture
-            apertures = CircularAperture(
-                (position_arr[i][0] + 1, position_arr[i][1] + 1), r=(fwhm_arr[i] / 2))
-            apertures.plot(ax, color='r', lw=1)
-            # Centroid
-            ax.plot(position_arr[i][0] + 1, position_arr[i][1] + 1, 'r+')
-            # Settings
-            ax.tick_params(
-                which='major', direction='in', top=True, right=True, color='w', length=5, 
-                width=1, labelsize=12)
-            ax.annotate(
-                'FWHM$=' + f'{fwhm_arr[i]:.2f}' + '\\,$px', xy=(0.05, 0.85), 
-                xycoords='axes fraction', color='w', fontsize=12)
-        fig.supxlabel('column', fontsize=16)
-        fig.supylabel('row', fontsize=16)
-        fig.suptitle(title[1], fontsize=16)
-        fig.tight_layout()
+        fig_path = _validatePath(path, title[1], '.pdf')
+        with PdfPages(fig_path, keep_empty=False) as pdf:
 
-        if save: plt.savefig(fig_path[1], dpi=100)
+            for i in range(n_peak):
 
-        if show: plt.show()
+                if fwhm_arr_masked.mask[i]:
+                    color = 'b'
+                else:
+                    color = 'r'
 
-        plt.close()
+                fig, ax = plt.subplots(1, 1, figsize=(3.2, 3.2), dpi=100)
+
+                # Image
+                _plot2d(
+                    ax=ax, ccd=cutout2d_arr[i], cmap='Greys_r', cbar=False, 
+                    xlabel='column', ylabel='row')
+                # Aperture
+                apertures = CircularAperture(
+                    (position_arr[i][0], position_arr[i][1]), r=(fwhm_arr[i] / 2))
+                apertures.plot(ax, color=color, lw=1)
+                # Centroid
+                ax.plot(position_arr[i][0], position_arr[i][1], '+', color=color, ms=15)
+                
+                # Settings
+                ax.tick_params(
+                    which='major', direction='in', top=True, right=True, color='w', 
+                    length=5, width=1, labelsize=12)
+                ax.annotate(
+                    'FWHM$=' + f'{fwhm_arr[i]:.2f}' + '\\,$px', xy=(0.05, 0.85), 
+                    xycoords='axes fraction', color='w', fontsize=12)
+                ax.set_title(f'cutoff at ({x[i]:.0f}, {y[i]:.0f})', fontsize=16)
+                fig.tight_layout()
+
+                pdf.savefig(fig, dpi=100)
+
+                plt.close()
     
     return fwhm, fwhm_err
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/modeling/core.py` & `astro-drpy-0.0.1.7/src/drpy/modeling/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 # NumPy
 import numpy as np
 # Astropy
 from astropy.stats import sigma_clip
+from astropy.utils.exceptions import AstropyUserWarning
 # SciPy
 from scipy import interpolate
 from scipy.ndimage import gaussian_filter
 # drpy
+from drpy.decorate import ignoreWarning
 from drpy.validate import _validateBool, _validateInteger, _validate1DArray
 
+sigma_clip = ignoreWarning(sigma_clip, 'ignore', AstropyUserWarning)
+
 __all__ = ['Poly1D', 'Spline1D', 'Spline2D', 'GaussianSmoothing2D']
 
 
-def Poly1D(x, y, weight=None, mask=None, degree=1, n_iter=5, sigma_lower=None, 
-           sigma_upper=None, grow=False, use_relative=False):
+def Poly1D(x, y, w=None, m=None, deg=1, maxiters=5, sigma_lower=None, sigma_upper=None, 
+           grow=False, use_relative=False):
     """Fit 1-dimensional polynomial function.
     
     Sigma clipping is used to mask bad data points.
 
     Parameters
     ----------
     x : array_like
         Input dimension of data points – must be increasing.
 
     y : array_like
         Input dimension of data points.
 
-    weight : array_like, optional
+    w : array_like, optional
         Weights for polynomial fitting. Must be positive. If `None` (default), weights 
         are all equal.
 
-    mask : array_like, optional
+    m : array_like, optional
         Initial mask for polynomial fitting. If `None` (default), data points are all 
         unmasked.
 
-    degree : int, optional
+    deg : int, optional
         Degree of the fitting polynomial.
         Default is `1`.
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be ``n_iter`` >= `0`.
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -71,74 +77,77 @@
     threshold_upper : scalar or `None`
         Upper threshold for clipping.
 
     master_mask : `~numpy.ndarray`
         Final mask after clipping.
     """
 
-    if weight is None:
-        weight = np.ones_like(y)
+    if w is None:
+        w = np.ones_like(y)
 
-    if mask is None:
-        mask = np.zeros_like(y, dtype=bool)
+    if m is None:
+        m = np.zeros_like(y, dtype=bool)
 
-    _validateInteger(n_iter, 'n_iter', (0, None), (True, None))
+    _validateInteger(maxiters, 'maxiters', (0, None), (True, None))
 
     _validateBool(use_relative, 'use_relative')
 
-    # Polynomial fitting iteratively (!!! only ``n_iter`` effective iterations !!!)
-    master_mask = mask & True
-    for k in range(n_iter + 1):
-
-        p = np.poly1d(
-            np.polyfit(x[~master_mask], y[~master_mask], degree, w=weight[~master_mask])
-        )
+    # Polynomial fitting iteratively
+    mask_new = m.copy()
+    mask_old = np.ones_like(mask_new, dtype=bool)
+    k = 0
+    while np.any(mask_new != mask_old) & (k <= maxiters):
+
+        mask_old = mask_new.copy()
+
+        p = np.poly1d(np.polyfit(x[~mask_old], y[~mask_old], deg=deg, w=w[~mask_old]))
 
         y_fit = p(x)
 
-        # Residual
-        residual = y - y_fit
+        # Standardized residual
+        residual = (y - y_fit) * w
         if use_relative:
             residual /= y_fit
 
         # Sigma clipping
-        if n_iter == 0:
+        if maxiters == 0:
             threshold_lower, threshold_upper = None, None
 
-        elif k < n_iter:
-            residual[mask] = np.nan
+        elif k < maxiters:
+            residual[m] = np.nan
             residual_masked, threshold_lower, threshold_upper = sigma_clip(
-                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper,
-                maxiters=1, stdfunc='std', axis=None, masked=True, return_bounds=True, 
-                grow=grow)
-            master_mask = residual_masked.mask
+                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+                maxiters=1, stdfunc='mad_std', axis=None, masked=True, 
+                return_bounds=True, grow=grow)
+            mask_new = residual_masked.mask
 
-    return p, residual, threshold_lower, threshold_upper, master_mask
+        k += 1
 
+    return p, residual, threshold_lower, threshold_upper, mask_new
 
-def Spline1D(x, y, weight=None, mask=None, order=3, n_piece=1, bbox=[None, None], 
-             n_iter=5, sigma_lower=None, sigma_upper=None, grow=False, 
-             use_relative=False):
+
+def Spline1D(x, y, w=None, m=None, order=3, n_piece=1, bbox=[None, None], maxiters=5, 
+             sigma_lower=None, sigma_upper=None, grow=False, use_relative=False):
     """Fit 1-dimensional spline function.
     
     Knots are set equally spaced. Sigma clipping is used to mask bad data points.
 
     Parameters
     ----------
     x : array_like
         Input dimension of data points – must be increasing.
 
     y : array_like
         Input dimension of data points.
 
-    weight : array_like, optional
+    w : array_like, optional
         Weights for spline fitting. Must be positive. If `None` (default), weights are 
         all equal.
 
-    mask : array_like, optional
+    m : array_like, optional
         Initial mask for spline fitting. If `None` (default), data points are all 
         unmasked.
 
     order : int, optional
         Degree of the smoothing spline. Must be `5` >= ``order`` >= `1`.
         Default is `3`, a cubic spline.
 
@@ -146,16 +155,18 @@
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is `1`.
 
     bbox : array_like, optional
         2-sequence specifying the boundary of the approximation interval. If `None` 
         (default), bbox = [x[0], x[-1]].
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be ``n_iter`` >= `0`.
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -184,62 +195,67 @@
     threshold_upper : scalar or `None`
         Upper threshold for in clipping.
 
     master_mask : `~numpy.ndarray`
         Final mask after clipping.
     """
 
-    if weight is None:
-        weight = np.ones_like(y)
+    if w is None:
+        w = np.ones_like(y)
 
-    if mask is None:
-        mask = np.zeros_like(y, dtype=bool)
+    if m is None:
+        m = np.zeros_like(y, dtype=bool)
 
     _validateInteger(n_piece, 'n_piece', (1, None), (True, None))
 
-    _validateInteger(n_iter, 'n_iter', (0, None), (True, None))
+    _validateInteger(maxiters, 'maxiters', (0, None), (True, None))
 
     _validateBool(use_relative, 'use_relative')
 
     # Set ``n_piece`` equally spaced knots
-    knots = x[~mask][0] \
-            + np.arange(1, n_piece) * (x[~mask][-1] - x[~mask][0]) / n_piece
+    knots = x[~m][0] + np.arange(1, n_piece) * (x[~m][-1] - x[~m][0]) / n_piece
 
     # Spline fitting iteratively
-    master_mask = mask & True
-    # !!! only ``n_iter`` effective iterations !!!
-    for k in range(n_iter + 1):
+    mask_new = m.copy()
+    mask_old = np.ones_like(mask_new, dtype=bool)
+    k = 0
+    while np.any(mask_new != mask_old) & (k <= maxiters):
+
+        mask_old = mask_new.copy()
+
         spl = interpolate.LSQUnivariateSpline(
-            x=x[~master_mask], y=y[~master_mask], t=knots, w=weight[~master_mask],
-            bbox=bbox, k=order, ext='extrapolate', check_finite=False)
+            x=x[~mask_old], y=y[~mask_old], t=knots, w=w[~mask_old], bbox=bbox, 
+            k=order, ext='extrapolate', check_finite=False)
 
         y_fit = spl(x)
 
-        # Residual
-        residual = y - y_fit
+        # Standardized residual
+        residual = (y - y_fit) * w
         if use_relative:
             residual /= y_fit
 
         # Sigma clipping
-        if n_iter == 0:
+        if maxiters == 0:
             threshold_lower, threshold_upper = None, None
 
-        elif k < n_iter:
-            residual[mask] = np.nan
+        elif k < maxiters:
+            residual[m] = np.nan
             residual_masked, threshold_lower, threshold_upper = sigma_clip(
-                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper,
-                maxiters=1, stdfunc='std', axis=None, masked=True, return_bounds=True, 
-                grow=grow)
-            master_mask = residual_masked.mask
+                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+                maxiters=1, stdfunc='mad_std', axis=None, masked=True, 
+                return_bounds=True, grow=grow)
+            mask_new = residual_masked.mask
 
-    return spl, residual, threshold_lower, threshold_upper, master_mask
+        k += 1
 
+    return spl, residual, threshold_lower, threshold_upper, mask_new
 
-def Spline2D(x, y, z, weight=None, mask=None, order=(3, 3), n_piece=(1, 1), 
-             bbox=[None, None, None, None], n_iter=5, sigma_lower=None, 
+
+def Spline2D(x, y, z, w=None, m=None, order=(3, 3), n_piece=(1, 1), 
+             bbox=[None, None, None, None], maxiters=5, sigma_lower=None, 
              sigma_upper=None, axis=None, grow=False, use_relative=False):
     """Fit 2-dimensional spline function.
     
     Knots are set equally spaced. Sigma clipping is used to mask bad data points.
 
     Parameters
     ----------
@@ -248,19 +264,19 @@
 
     y : array_like
         Input dimension of data points.
 
     z : array_like
         Input dimension of data points.
 
-    weight : array_like or `None`, optional
+    w : array_like or `None`, optional
         Weights for spline fitting. Must be positive. If `None` (default), weights are 
         all equal.
 
-    mask : array_like or `None`, optional
+    m : array_like or `None`, optional
         Initial mask for spline fitting. If `None` (default), data points are all 
         unmasked.
 
     order : 2-tuple of int, optional
         Degree of the smoothing spline. Must be `5` >= ``order`` >= `1`.
         Default is (3, 3).
 
@@ -268,16 +284,18 @@
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is (1, 1).
         
     bbox : array_like, optional
         Sequence of length 4 specifying the boundary of the rectangular approximation 
         domain. By default, bbox=[x[0], x[-1], y[0], y[-1]].
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be ``n_iter`` >= `0`. 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -312,72 +330,75 @@
     threshold_upper : scalar or array_like or None
         Upper threshold for clipping.
     
     master_mask : `~numpy.ndarray`
         Final mask after clipping.
     """
 
-    if weight is None:
-        weight = np.ones_like(z)
+    if w is None:
+        w = np.ones_like(z)
 
-    if mask is None:
-        mask = np.zeros_like(z, dtype=bool)
+    if m is None:
+        m = np.zeros_like(z, dtype=bool)
 
     _validate1DArray(order, 'order', 2, True)
 
     _validate1DArray(n_piece, 'n_piece', 2, True)
     _validateInteger(n_piece[0], 'n_piece[0]', (1, None), (True, None))
     _validateInteger(n_piece[1], 'n_piece[1]', (1, None), (True, None))
 
-    _validateInteger(n_iter, 'n_iter', (0, None), (True, None))
+    _validateInteger(maxiters, 'maxiters', (0, None), (True, None))
 
     _validateBool(use_relative, 'use_relative')
 
     # Order
     xorder, yorder = order
 
     # Set equally spaced knots
     xpiece, ypiece = n_piece
-    xknots = x[~mask][0] \
-             + np.arange(1, xpiece) * (x[~mask][-1] - x[~mask][0]) / xpiece
-    yknots = y[~mask][0] \
-             + np.arange(1, ypiece) * (y[~mask][-1] - y[~mask][0]) / ypiece
+    xknots = x[~m][0] + np.arange(1, xpiece) * (x[~m][-1] - x[~m][0]) / xpiece
+    yknots = y[~m][0] + np.arange(1, ypiece) * (y[~m][-1] - y[~m][0]) / ypiece
     
-    # 2-dimensional spline fitting iteratively (!!! only ``n_iter`` effective 
-    # iterations !!!)
-    master_mask = mask & True
-    for k in range(n_iter + 1):
+    # 2-dimensional spline fitting iteratively
+    mask_new = m.copy()
+    mask_old = np.ones_like(mask_new, dtype=bool)
+    k = 0
+    while np.any(mask_new != mask_old) & (k <= maxiters):
+
+        mask_old = mask_new.copy()
+
         bispl = interpolate.LSQBivariateSpline(
-            x=x[~master_mask], y=y[~master_mask], z=z[~master_mask], tx=xknots, 
-            ty=yknots, w=weight[~master_mask], bbox=bbox, kx=xorder, ky=yorder, 
-            eps=None)
+            x=x[~mask_old], y=y[~mask_old], z=z[~mask_old], tx=xknots, ty=yknots, 
+            w=w[~mask_old], bbox=bbox, kx=xorder, ky=yorder, eps=None)
 
         z_fit = bispl(x.flatten(), y.flatten(), grid=False).reshape(x.shape)
 
-        # Residual
-        residual = z - z_fit
+        # Standardized residual
+        residual = (z - z_fit) * w
         if use_relative:
             residual /= z_fit
 
         # Sigma clipping
-        if n_iter == 0:
+        if maxiters == 0:
             threshold_lower, threshold_upper = None, None
 
-        elif k < n_iter:
-            residual[mask] = np.nan
+        elif k < maxiters:
+            residual[m] = np.nan
             residual_masked, threshold_lower, threshold_upper = sigma_clip(
-                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper,
-                maxiters=1, stdfunc='std', axis=axis, masked=True, return_bounds=True, 
-                grow=grow)
-            master_mask = residual_masked.mask
+                data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+                maxiters=1, stdfunc='mad_std', axis=axis, masked=True, 
+                return_bounds=True, grow=grow)
+            mask_new = residual_masked.mask
 
-    return bispl, residual, threshold_lower, threshold_upper, master_mask
+        k += 1
 
+    return bispl, residual, threshold_lower, threshold_upper, mask_new
 
-def GaussianSmoothing2D(x, y, z, sigma, mask=None, n_iter=5, sigma_lower=None, 
+
+def GaussianSmoothing2D(x, y, z, sigma, m=None, maxiters=5, sigma_lower=None, 
                         sigma_upper=None, axis=None, grow=False, use_relative=False):
     """2-dimensional Gaussian smoothing.
 
     Parameters
     ----------
     x : array_like
         Input dimension of data points.
@@ -389,20 +410,22 @@
         Input dimension of data points.
 
     sigma : scalar or sequence of scalars
         Standard deviation for Gaussian kernel. The standard deviations of the Gaussian 
         filter are given for each axis as a sequence, or as a single number, in which 
         case it is equal for both axes.
 
-    mask : array_like, optional
+    m : array_like, optional
         Initial mask for Gaussian smoothing. If `None` (default), data points are all 
         unmasked.
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be ``n_iter`` >= `0`.
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -437,45 +460,51 @@
     threshold_upper : scalar or array_like or None
         Upper threshold for clipping.
 
     master_mask : `~numpy.ndarray`
         Final mask after clipping.
     """
 
-    if mask is None:
-        mask = np.zeros(z.shape, dtype=bool)
+    if m is None:
+        m = np.zeros(z.shape, dtype=bool)
 
-    _validateInteger(n_iter, 'n_iter', (0, None), (True, None))
+    _validateInteger(maxiters, 'maxiters', (0, None), (True, None))
 
     _validateBool(use_relative, 'use_relative')
 
-    # Convolve with Gaussian kernel iteratively (!!! only ``n_iter`` effective 
-    # iterations !!!)
-    master_mask = mask & True
-    for k in range(n_iter + 1):
+    # Convolve with Gaussian kernel iteratively
+    mask_new = m.copy()
+    mask_old = np.ones_like(mask_new, dtype=bool)
+    k = 0
+    while np.any(mask_new != mask_old) & (k <= maxiters):
+
+        mask_old = mask_new.copy()
+
         # Interpolate
         interpolated_z = interpolate.griddata(
-            points=(x[~master_mask], y[~master_mask]), values=z[~master_mask],
+            points=(x[~mask_old], y[~mask_old]), values=z[~mask_old],
             xi=(x.flatten(), y.flatten()), method='nearest').reshape(x.shape)
 
         # Smooth
         z_smoothed = gaussian_filter(
             input=interpolated_z, sigma=sigma, order=0, mode='reflect')
 
         # Residual
         residual = z - z_smoothed
         if use_relative:
             residual /= z_smoothed
 
         # Sigma clipping
-        if n_iter == 0:
+        if maxiters == 0:
             threshold_lower, threshold_upper = None, None
 
-        elif k < n_iter:
-            residual[mask] = np.nan
+        elif k < maxiters:
+            residual[m] = np.nan
             residual_masked, threshold_lower, threshold_upper = sigma_clip(
                 data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper,
-                maxiters=1, stdfunc='std', axis=axis, masked=True, return_bounds=True,
-                grow=grow)
-            master_mask = residual_masked.mask
+                maxiters=1, stdfunc='mad_std', axis=axis, masked=True, 
+                return_bounds=True, grow=grow)
+            mask_new = residual_masked.mask
+
+        k += 1
 
-    return z_smoothed, residual, threshold_lower, threshold_upper, master_mask
+    return z_smoothed, residual, threshold_lower, threshold_upper, mask_new
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/modeling/function.py` & `astro-drpy-0.0.1.7/src/drpy/modeling/function.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/center.py` & `astro-drpy-0.0.1.7/src/drpy/onedspec/center.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,16 @@
             x = index[left_bases[i]:right_bases[i]]
             y = spectrum[left_bases[i]:right_bases[i]]
 
             try:
                 center = _center1D_Gaussian(x, y, initial_guess, 0)
                 refined_index.append(i); refined_peaks.append(center)
 
-            except (RuntimeError, TypeError, OptimizeWarning): # raise exception here
+            # raise exception here
+            except (RuntimeError, TypeError, ValueError, OptimizeWarning):
                 pass
 
     refined_index = np.array(refined_index)
     refined_peaks = np.array(refined_peaks)
 
     # Mask peaks that are close from each other
     mask = np.isclose(refined_peaks[:-1], refined_peaks[1:], rtol=0, atol=tolerance)
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/core.py` & `astro-drpy-0.0.1.7/src/drpy/onedspec/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,32 +7,323 @@
 # matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.patches import Rectangle
 from matplotlib.collections import PatchCollection
 # AstroPy
 import astropy.units as u
 from astropy.time import Time
-from astropy.table import Table
+from astropy.table import QTable
 from astropy.nddata import StdDevUncertainty
 # specutils
 from specutils import Spectrum1D
 # drpy
 from drpy import conf
-from drpy.modeling import Poly1D, Spline1D, Spline2D, GaussianSmoothing2D
+from drpy.modeling import Poly1D, Spline1D
 from drpy.plotting import plotFitting, _plotSpectrum1D
-from drpy.validate import (_validateBool, _validateString, _validateSpectrum, 
-                           _validatePath)
+from drpy.validate import (_validateBool, _validateString, _validateInteger, 
+                           _validateSpectrum, _validatePath)
 
 from .center import _center1D_Gaussian, _refinePeakBases, _refinePeaks
 from .io import loadSpectrum1D, loadStandardSpectrum, loadExtinctionCurve
 
 __all__ = ['dispcor', 'sensfunc', 'calibrate1d']
 
 
-def dispcor(spectrum1d, reverse, reference, n_piece=3, refit=True, n_iter=5, 
+def dispcor(spectrum1d, reverse, reference, n_sub=20, refit=True, prominence=1e-3, 
+            degree=1, maxiters=5, sigma_lower=None, sigma_upper=None, grow=False, 
+            use_mask=False, title='dispcor', show=conf.fig_show, save=conf.fig_save, 
+            path=conf.fig_path, **kwargs):
+    """Dispersion correction.
+
+    Parameters
+    ----------
+    spectrum1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
+        Input spectrum.
+
+    reverse : bool
+        Reverse the input spectrum or not. Set to `True` if the spectral axis of the 
+        input spectrum is in reverse order.
+
+    reference : `~specutils.Spectrum1D` or str
+        File name of the reference spectrum.
+
+    n_sub : int
+        A pixel is divided into ``n_sub`` subpixels before cross-correlation.
+        Default is `20`.
+
+    refit : bool, optional
+        Refit the dispersion solution or not. If `True`, lines in the input spectrum 
+        are recentered and then used to fit the dispersion solution.
+
+    degree : int, optional
+        Degree of the fitting polynomial.
+        Default is `3`.
+
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
+        Default is `5`.
+
+    sigma_lower : scalar or `None`, optional
+        Number of standard deviations to use as the lower bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    sigma_upper : scalar or `None`, optional
+        Number of standard deviations to use as the upper bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    grow : float or `False`, optional
+        Radius within which to mask the neighbouring pixels of those that fall outwith 
+        the clipping limits (only applied along axis, if specified).
+
+    use_mask : bool, optional
+        If `True` and a mask array is attributed to ``spectrum1d``, the masked pixels are 
+        interpolated before cross-correlation. 
+        Default is `False`.
+
+    Returns
+    -------
+    new_spectrum1d : `~specutils.Spectrum1D`
+        Dispersion corrected spectrum.
+    """
+    
+    
+    new_spectrum1d, _, flux, _, mask = _validateSpectrum(
+        spectrum1d, 'spectrum1d', False, use_mask)
+
+    # ``flux`` and ``mask`` may be 2-dimensional arrays, though each one may only have 
+    # one row. Use flatten to get rid of the additional dimension.
+    if flux.ndim > 1:
+        flux = flux.flatten()[:flux.shape[-1]]
+        mask = mask.flatten()[:mask.shape[-1]]
+
+    index = np.arange(flux.shape[0])
+
+    # Interpolate bad pixels
+    flux = interpolate.interp1d(
+        index[~mask], flux[~mask], bounds_error=False, fill_value='extrapolate', 
+        assume_sorted=True)(index)
+
+    flux /= np.nanmax(flux)
+    
+    _validateBool(reverse, 'reverse')
+
+    if reverse:
+        flux = flux[::-1]
+
+    # Parse reference spectrum
+    if isinstance(reference, Spectrum1D):
+        spectrum1d_ref = deepcopy(reference)
+    else:
+        spectrum1d_ref = loadSpectrum1D(reference, ext='spec')
+    spectral_axis_ref = spectrum1d_ref.spectral_axis.value
+    unit_spectral_axis = spectrum1d_ref.spectral_axis.unit
+    flux_ref = spectrum1d_ref.flux.value
+    flux_ref /= np.nanmax(flux_ref)
+
+    n_pix = spectral_axis_ref.shape[0]
+
+    index_ref = np.arange(n_pix)
+
+    n_sub = _validateInteger(n_sub, 'n_sub', (1, None), (True, None))
+
+    # Of type `~numpy.float64`, although still named as an index array.
+    index_dense = np.linspace(0, index[-1], index[-1] * n_sub + 1)
+    flux_dense = interpolate.interp1d(index, flux, assume_sorted=True)(index_dense)
+
+    # Of type `~numpy.float64`, although still named as an index array.
+    index_ref_dense = np.linspace(0, index_ref[-1], index_ref[-1] * n_sub + 1)
+    flux_ref_dense = interpolate.interp1d(
+        index_ref, flux_ref, assume_sorted=True)(index_ref_dense)
+
+    # Here assumes that the zeropoint shift is no more than ±(n/4)
+    n_ext = index_ref[-1] // 4
+
+    # Reference spectrum
+    index_ref_dense_ext = np.linspace(
+        0, index_ref[-1] + 2 * n_ext, (index_ref[-1] + 2 * n_ext) * n_sub + 1) - n_ext
+    flux_ref_dense_ext = np.hstack([
+        flux_ref_dense[-n_ext * n_sub:], flux_ref_dense, flux_ref_dense[:n_ext * n_sub]
+    ])
+
+    # Get zeropoint shift through cross-correlation
+    index_max = signal.correlate(
+        flux_ref_dense_ext, flux_dense, mode='valid', method='auto').argmax()
+    # The shift value is just the index of the maximum in the ``index_ref_dense_ext``
+    delta = index_ref_dense_ext[index_max]
+
+    _validateBool(refit, 'refit')
+
+    if refit:
+
+        # Find peaks in the reference spectrum
+        peaks, properties = signal.find_peaks(
+            x=flux_ref, prominence=prominence, **kwargs)
+        # Refine peaks in the reference spectrum
+        heights = flux_ref[peaks]
+        refined_left_bases, refined_right_bases = _refinePeakBases(
+            peaks=peaks, left_bases=properties['left_bases'], 
+            right_bases=properties['right_bases'], n_peak=peaks.shape[0], copy=True)
+        refined_peaks_ref, refined_index_ref = _refinePeaks(
+            flux_ref, peaks, heights, refined_left_bases, refined_right_bases, 1)
+    
+        # Reidentify in the input spectrum
+        shifted_peaks = refined_peaks_ref - delta
+        shifted_left_bases = refined_left_bases[refined_index_ref] - delta
+        shifted_right_bases = refined_right_bases[refined_index_ref] - delta
+        refined_peaks, refined_index = _refinePeaks(
+            flux, shifted_peaks, heights[refined_index_ref], shifted_left_bases, 
+            shifted_right_bases, 1)
+
+        # Fit polynomial
+        delta_peaks = refined_peaks_ref[refined_index] - refined_peaks
+        spl, residual, threshold_lower, threshold_upper, master_mask = Poly1D(
+            x=refined_peaks, y=delta_peaks, deg=degree, maxiters=maxiters, 
+            sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
+            use_relative=False)
+        delta = spl(index)
+
+        rms = np.sqrt((residual[~master_mask]**2).sum() / (~master_mask).sum())
+
+        # print(f'dispersion solution rms = {rms:.3}')
+
+        plotFitting(
+            x=refined_peaks, y=delta_peaks, m=master_mask, x_fit=index, y_fit=delta, 
+            r=residual, threshold_lower=threshold_lower, 
+            threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
+            ylabel='difference [px]', title='dispcor', show=show, save=save, 
+            path=path, use_relative=False)
+
+    # !!! The extrapolated wavelengths are not reliable !!!
+    spectral_axis = interpolate.interp1d(
+        index_ref, spectral_axis_ref, bounds_error=False, fill_value='extrapolate', 
+        assume_sorted=True)(index + delta)
+
+    # Plot
+    _validateBool(show, 'show')
+    _validateBool(save, 'save')
+
+    if show | save:
+
+        # Peak detection plot
+        title = 'dispcor peak detection'
+
+        # Split into subplots
+        n_subplot = 2
+
+        fig, ax = plt.subplots(n_subplot, 1, dpi=100)
+
+        length = n_pix // n_subplot + 1
+        for i in range(n_subplot):
+
+            idx_start, idx_end = i * length, (i + 1) * length
+            idx_peak = np.where(
+                (idx_start <= refined_peaks_ref[refined_index]) 
+                & (refined_peaks_ref[refined_index] < idx_end))[0]
+
+            ax[i].step(
+                index_ref[idx_start:idx_end], flux_ref[idx_start:idx_end], color='k', 
+                ls='-', where='mid')
+            for idx in idx_peak:
+                ymin = heights[refined_index][idx] * 1.2
+                ymax = heights[refined_index][idx] * 1.5
+                ax[i].plot(
+                    [refined_peaks_ref[refined_index][idx], 
+                     refined_peaks_ref[refined_index][idx]], [ymin, ymax], 'r-', 
+                    lw=1.5)
+
+            # Settings
+            ax[i].grid(axis='both', color='0.95', zorder=-1)
+            ax[i].set_xlim(idx_start, idx_end)
+            ax[i].set_yscale('log')
+            ax[i].tick_params(
+                which='major', direction='in', top=True, right=True, length=5, 
+                width=1.5, labelsize=12)
+            ax[i].tick_params(
+                which='minor', direction='in', top=True, right=True, length=3, 
+                width=1.5, labelsize=12)
+            ax[i].set_ylabel('normalized intensity', fontsize=16)
+        ax[-1].set_xlabel('dispersion axis [px]', fontsize=16)
+        ax[0].set_title(title, fontsize=16)
+        fig.align_ylabels()
+        fig.set_figheight(fig.get_figwidth() * n_subplot / 2)
+        fig.tight_layout()
+
+        # Save
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
+        
+        if show:
+            plt.show()
+
+        plt.close()
+
+        _validateString(title, 'title')
+        if title != 'dispcor':
+            title = f'{title} dispcor'
+
+        xlabel = f'spectral axis [{unit_spectral_axis.to_string()}]'
+
+        fig, ax = plt.subplots(1, 1, dpi=100)
+
+        # Spectrum
+        ax.step(
+            spectral_axis, flux + 1, where='mid', color='C0', zorder=3, label='custom')
+        ax.step(
+            spectral_axis_ref, flux_ref, where='mid', color='C1', zorder=3, 
+            label='reference')
+
+        # Settings
+        ax.grid(axis='both', color='0.95', zorder=-1)
+        ax.set_xlim(spectral_axis[0], spectral_axis[-1])
+        ax.tick_params(
+            which='major', direction='in', top=True, right=True, length=5, width=1.5, 
+            labelsize=12)
+        ax.set_xlabel(xlabel, fontsize=16)
+        ax.set_ylabel('flux', fontsize=16)
+        ax.legend(fontsize=16)
+        ax.set_title(title, fontsize=16)
+        fig.set_figheight(fig.get_figwidth() * 2 / 3)
+        fig.tight_layout()
+        
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
+
+        if show:
+            plt.show()
+
+        plt.close()
+
+    if reverse:
+        spectral_axis = spectral_axis[::-1]
+
+    spectral_axis *= unit_spectral_axis
+
+    if 'header' in new_spectrum1d.meta:
+        meta = new_spectrum1d.meta.copy()
+
+    else:
+        meta = {'header': dict()}
+
+    meta['header']['DISPCOR'] = ('{} Dispersion correction.'.format(
+        Time.now().to_value('iso', subfmt='date_hm')))
+
+    # Output
+    # `__setattr__` of `~specutils.Spectrum1D` is disabled
+    new_spectrum1d = Spectrum1D(
+        spectral_axis=spectral_axis, flux=new_spectrum1d.flux, 
+        uncertainty=new_spectrum1d.uncertainty, mask=new_spectrum1d.mask, meta=meta)
+
+    return new_spectrum1d
+
+
+def _dispcor(spectrum1d, reverse, reference, n_piece=3, refit=True, maxiters=5, 
             sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
             title='dispcor', show=conf.fig_show, save=conf.fig_save, 
             path=conf.fig_path):
     """Dispersion correction.
 
     Parameters
     ----------
@@ -50,14 +341,32 @@
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is `3`.
 
     refit : bool, optional
         Refit the dispersion solution or not. If `True`, lines in the input spectrum 
         are recentered and then used to fit the dispersion solution.
 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
+        Default is `5`.
+
+    sigma_lower : scalar or `None`, optional
+        Number of standard deviations to use as the lower bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    sigma_upper : scalar or `None`, optional
+        Number of standard deviations to use as the upper bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    grow : float or `False`, optional
+        Radius within which to mask the neighbouring pixels of those that fall outwith 
+        the clipping limits (only applied along axis, if specified).
+
     use_mask : bool, optional
         If `True` and a mask array is attributed to ``spectrum1d``, the masked pixels are 
         interpolated before cross-correlation. 
         Default is `False`.
 
     Returns
     -------
@@ -129,15 +438,15 @@
         # !!! The extrapolated wavelengths are not reliable !!!
         spectral_axis = interpolate.interp1d(
             index_ref, spectral_axis_ref, bounds_error=False, fill_value='extrapolate', 
             assume_sorted=True)(index + shift)
 
     else:
         # Load peak table
-        peak_tbl = Table.read(reference, format='fits', hdu='peak')
+        peak_tbl = QTable.read(reference, format='fits', hdu='peak')
 
         # Reidentify
         shifted_peaks = peak_tbl['peaks'].value - shift
         shifted_left_bases = peak_tbl['left_bases'].value - shift
         shifted_right_bases = peak_tbl['right_bases'].value - shift
         heights = peak_tbl['heights'].value
         
@@ -147,41 +456,41 @@
 
         refined_peaks, refined_index = _refinePeaks(
             flux, shifted_peaks, heights, refined_left_bases, refined_right_bases, 1)
 
         # Fit cubic spline function
         spectral_axis_peaks = peak_tbl['spectral_axis'].value[refined_index]
         spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
-            x=refined_peaks, y=spectral_axis_peaks, weight=None, mask=None, order=3, 
-            n_piece=n_piece, n_iter=n_iter, sigma_lower=sigma_lower, 
-            sigma_upper=sigma_upper, grow=grow, use_relative=False)
+            x=refined_peaks, y=spectral_axis_peaks, order=3, n_piece=n_piece, 
+            maxiters=maxiters, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
+            use_relative=False)
         spectral_axis = spl(index)
 
         rms = np.sqrt((residual[~master_mask]**2).sum() / (~master_mask).sum())
 
         print(f'dispersion solution rms = {rms:.3}')
 
         plotFitting(
-            x=spectral_axis_peaks, y=refined_peaks, residual=residual, 
-            mask=master_mask, x_fit=spectral_axis, y_fit=index, 
-            threshold_lower=threshold_lower, threshold_upper=threshold_upper, 
+            x=spectral_axis_peaks, y=refined_peaks, m=master_mask, x_fit=spectral_axis, 
+            y_fit=index, r=residual, threshold_lower=threshold_lower, 
+            threshold_upper=threshold_upper, 
             xlabel=f'spectral axis [{unit_spectral_axis.to_string()}]', 
             ylabel='dispersion axis [px]', title='dispersion solution', show=show, 
             save=save, path=path, use_relative=False)
 
+    # Plot
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-    if title != 'dispcor':
-        title = f'{title} dispcor'
-
-    fig_path = _validatePath(save, path, title)
+    _validateBool(save, 'save')
 
     if show | save:
 
+        _validateString(title, 'title')
+        if title != 'dispcor':
+            title = f'{title} dispcor'
+
         xlabel = f'spectral axis [{unit_spectral_axis.to_string()}]'
 
         fig, ax = plt.subplots(1, 1, dpi=100)
 
         # Spectrum
         ax.step(
             spectral_axis, flux + 1, where='mid', color='C0', zorder=3, label='custom')
@@ -198,27 +507,30 @@
         ax.set_xlabel(xlabel, fontsize=16)
         ax.set_ylabel('flux', fontsize=16)
         ax.legend(fontsize=16)
         ax.set_title(title, fontsize=16)
         fig.set_figheight(0.5 * fig.get_figwidth())
         fig.tight_layout()
         
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
     if reverse:
         spectral_axis = spectral_axis[::-1]
 
     spectral_axis *= unit_spectral_axis
 
     if 'header' in new_spectrum1d.meta:
-        meta = deepcopy(new_spectrum1d.meta)
+        meta = new_spectrum1d.meta.copy()
 
     else:
         meta = {'header': dict()}
 
     meta['header']['DISPCOR'] = ('{} Dispersion correction.'.format(
         Time.now().to_value('iso', subfmt='date_hm')))
 
@@ -228,19 +540,19 @@
         spectral_axis=spectral_axis, flux=new_spectrum1d.flux, 
         uncertainty=new_spectrum1d.uncertainty, mask=new_spectrum1d.mask, meta=meta)
 
     return new_spectrum1d
 
 
 def sensfunc(spectrum1d, exptime, airmass, extinct, standard, bandwid=None, 
-             bandsep=None, n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, 
+             bandsep=None, n_piece=3, maxiters=5, sigma_lower=None, sigma_upper=None, 
              grow=False, use_mask=False, title='sensfunc', show=conf.fig_show, 
              save=conf.fig_save, path=conf.fig_path):
     """Create sensitivity function.
-    
+
     Parameters
     ----------
     spectrum1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
         Input spectrum.
 
     exptime : str or scalar
         Exposure time. Should be either a keyword in the header (str) or exposure time 
@@ -261,16 +573,18 @@
     bandwid, bandsep : scalar or `None`, optional
         Bandpass widths and separations in wavelength units.
 
     n_piece : int, optional
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is `3`.
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`.
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -288,30 +602,30 @@
 
     Returns
     -------
     sens1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
         Sensitivity function.
     """
 
-    new_spectrum1d, _, flux_obs, _, mask_obs = _validateSpectrum(
+    new_spectrum1d, _, flux_obs, uncertainty_obs, mask_obs = _validateSpectrum(
         spectrum1d, 'spectrum1d', False, use_mask)
 
     if isinstance(exptime, str):
         exptime = spectrum1d.meta['header'][exptime]
 
     # ``flux`` and ``mask`` may be 2-dimensional arrays, though each one may only have 
     # one row. Use flatten to get rid of additional dimensions.
     if flux_obs.ndim > 1:
         flux_obs = flux_obs.flatten()[:flux_obs.shape[-1]]
         mask_obs = mask_obs.flatten()[:mask_obs.shape[-1]]
 
     flux_obs /= exptime
 
-    wavelength_obs = deepcopy(new_spectrum1d.wavelength.value)
-    bin_edges_obs = deepcopy(new_spectrum1d.bin_edges.to(u.AA).value)
+    wavelength_obs = new_spectrum1d.wavelength.value.copy()
+    bin_edges_obs = new_spectrum1d.bin_edges.to(u.AA).value.copy()
     bin_width_obs = np.diff(bin_edges_obs)
 
     # Check whether is reversed
     if wavelength_obs[0] > wavelength_obs[-1]:
         wavelength_obs = wavelength_obs[::-1] # [Angstrom]
         bin_edges_obs = bin_edges_obs[::-1]   # [Angstrom]
         bin_width_obs = -bin_width_obs[::-1]  # [Angstrom]
@@ -455,38 +769,36 @@
 
         sens += (airmass * extinction)
 
     mask_sens = np.isnan(sens) | mask_bp_obs
 
     # Fit cubic spline function
     spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
-        x=wavelength, y=sens, weight=None, mask=mask_sens, order=3, n_piece=n_piece, 
-        n_iter=n_iter, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
-        use_relative=False)
+        x=wavelength, y=sens, m=mask_sens, order=3, n_piece=n_piece, maxiters=maxiters, 
+        sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, use_relative=False)
 
     sens_fit = spl(wavelength_obs)
     # Use RMS as uncertainty
     uncertainty_sens_fit = np.full(n_obs, residual[~master_mask].std(ddof=1))
     
     out_of_range = (
         (wavelength_obs < wavelength[~master_mask][0]) | 
         (wavelength_obs > wavelength[~master_mask][-1])
     )
     sens_fit[out_of_range] = np.nan
     uncertainty_sens_fit[out_of_range] = np.nan
 
     # Plot
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-
-    fig_path = _validatePath(save, path, title)
+    _validateBool(save, 'save')
 
     if show | save:
 
+        _validateString(title, 'title')
+
         fig, ax = plt.subplots(1, 1, dpi=100)
 
         # Spectrum
         _plotSpectrum1D(
             ax, wavelength_obs, (flux_obs / bin_width_obs), xlabel='wavelength [A]')
 
         # Bandpasses
@@ -500,55 +812,58 @@
             patches.append(rectangle)
         patch_collection = PatchCollection(
             patches, facecolor='None', edgecolor='r', lw=1.5, zorder=2.5)
         ax.add_collection(patch_collection)
 
         # Settings
         ax.set_title(title, fontsize=16)
-        fig.set_figheight(fig.get_figwidth * 2 / 3)
+        fig.set_figheight(fig.get_figwidth() * 2 / 3)
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
+    # Sensitivity function fitting
     plotFitting(
-        x=wavelength, y=sens, residual=residual, mask=master_mask, 
-        x_fit=wavelength_obs, y_fit=sens_fit, threshold_lower=threshold_lower, 
-        threshold_upper=threshold_upper, xlabel='wavelength [A]', 
-        ylabel='sensitivity function', title=title, show=show, save=save, path=path, 
-        use_relative=False)
+        x=wavelength, y=sens, m=master_mask, x_fit=wavelength_obs, y_fit=sens_fit, 
+        r=residual, threshold_lower=threshold_lower, threshold_upper=threshold_upper, 
+        xlabel='wavelength [A]', ylabel='sensitivity function', title=title, show=show, 
+        save=save, path=path, use_relative=False)
 
     unit_sens_fit = new_spectrum1d.flux.unit / u.s / u.AA / spectrum_lib.flux.unit
 
     if isReversed:
         sens_fit = sens_fit[::-1] * unit_sens_fit
         uncertainty_sens_fit = StdDevUncertainty(uncertainty_sens_fit[::-1])
     else:
         sens_fit *= unit_sens_fit
         sens_fit_uncertainty = StdDevUncertainty(uncertainty_sens_fit)
 
     if 'header' in new_spectrum1d.meta:
-        meta = deepcopy(new_spectrum1d.meta)
+        meta = new_spectrum1d.meta.copy()
     else:
         meta = {'header': dict()}
     # Add headers here
     meta['header']['EXPTIME'] = exptime
     meta['header']['AIRMASS'] = airmass
     meta['header']['SENSFUNC'] = '{}'.format(
         Time.now().to_value('iso', subfmt='date_hm'))
 
     # Output
     sens1d = Spectrum1D(
         spectral_axis=new_spectrum1d.spectral_axis, flux=sens_fit, 
         uncertainty=uncertainty_sens_fit, meta=meta)
 
-    return sens1d
+    return sens1d, spl
 
 
 def calibrate1d(spectrum1d, exptime, airmass, extinct, sens1d, use_uncertainty=False):
     """Apply a flux calibration to 1-dimensional spectra.
     
     ``spectrum1d`` and ``sens1d`` are assumed to have the same spectral axis, including 
     values, units and order (reversed or not).
@@ -660,15 +975,15 @@
     calibrated_spectrum1d = new_spectrum1d / new_sens1d
     
     # Output
     if new_spectrum1d.uncertainty is None:
         calibrated_spectrum1d.uncertainty = None
 
     if 'header' in new_spectrum1d.meta:
-        meta = deepcopy(new_spectrum1d.meta)
+        meta = new_spectrum1d.meta.copy()
     else:
         meta = {'header': dict()}
     # Add headers here
     meta['header']['EXPTIME'] = exptime.value
     meta['header']['AIRMASS'] = airmass
     meta['header']['CALIBRAT'] = '{} Calibrated'.format(
         Time.now().to_value('iso', subfmt='date_hm'))
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/io.py` & `astro-drpy-0.0.1.7/src/drpy/onedspec/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from glob import glob
 
 # NumPy
 import numpy as np
 # AstroPy
 from astropy.io import fits
 from astropy.time import Time
-from astropy.table import Table
+from astropy.table import QTable
 import astropy.units as u
 from astropy.nddata import StdDevUncertainty
 # specutils
 from specutils import Spectrum1D
 # drpy
 from drpy.validate import _validateSpectrum1D
 
@@ -115,39 +115,33 @@
     spectrum1d : `~specutils.Spectrum1D`
         The loaded spectrum.
     """
 
     with fits.open(file_name, **kwargs) as hdulist:
         hdu = hdulist[ext]
         header = hdu.header
-        table = Table.read(hdu)
+        qtable = QTable.read(hdu)
 
-    spectral_axis = table['spectral_axis'].value * table['spectral_axis'].unit
-
-    flux = table['flux'].value * table['flux'].unit
-
-    colnames = table.colnames
-
-    if 'uncertainty' in colnames:
-        uncertainty = StdDevUncertainty(table['uncertainty'].value)
+    if 'uncertainty' in qtable.colnames:
+        uncertainty = StdDevUncertainty(qtable['uncertainty'].value.T)
 
     else:
         uncertainty = None
-    
-    if 'mask' in colnames:
-        mask = table['mask'].value
+
+    if 'mask' in qtable.colnames:
+        mask = qtable['mask'].value.T
 
     else:
         mask = None
 
     meta = {'header': header}
-    
+
     spectrum1d = Spectrum1D(
-        spectral_axis=spectral_axis, flux=flux, uncertainty=uncertainty, mask=mask, 
-        meta=meta)
+        spectral_axis=qtable['spectral_axis'], flux=qtable['flux'].T, 
+        uncertainty=uncertainty, mask=mask, meta=meta)
 
     return spectrum1d
 
 
 def _AB_to_flux(wavelength, AB):
     """Convert AB magnitude to flux in [erg/cm2/s/A].
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/README` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/README`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/h.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/h.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/i.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/i.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/j.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/j.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/k.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/k.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/l.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/l.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/m.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/m.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/params.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/params.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/r.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/r.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/u.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/u.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/v.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/blackbody/v.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/names.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/iidscal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/he3.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/he3.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/names.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/he3.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/he3.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/names.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/names.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat` & `astro-drpy-0.0.1.7/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/plotting.py` & `astro-drpy-0.0.1.7/src/drpy/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,53 +19,59 @@
 plt.rcParams['axes.linewidth'] = 1.5
 plt.rcParams['mathtext.fontset'] = 'stix'
 plt.rcParams['font.family'] = 'STIXGeneral'
 
 __all__ = ['plotFitting', 'plotSpectrum1D', 'plot2d']
 
 
-def _plotFitting(ax, x, y, residual, mask, y_fit, x_fit, threshold_lower, 
-                 threshold_upper, xlabel='x', ylabel='y', use_relative=False):
+def _plotFitting(ax, x, y, m, x_fit, y_fit, r, threshold_lower, threshold_upper, 
+                 xlabel='x', ylabel='y', use_relative=False):
     """Plot fitting."""
 
+    # ymin_fit = np.nanmin(y_fit)
+    # ymax_fit = np.nanmax(y_fit)
+    # y_fit_range = ymax_fit - ymin_fit
+    # ymin_fit -= 0.1 * y_fit_range
+    # ymax_fit += 0.1 * y_fit_range
+
     if (threshold_lower is None) & (threshold_upper is None):
         ymin = None; ymax = None
     elif threshold_lower is None:
         ymax = 1.67 * threshold_upper; ymin = -ymax
     elif threshold_upper is None:
         ymin = 1.67 * threshold_lower; ymax = -ymin
     else:
         ymax = 1.67 * np.max(np.abs([threshold_lower, threshold_upper])); ymin = -ymax
-    
+
+    rms = np.sqrt((r[~m]**2).sum() / (~m).sum())
+
     # Data
-    ax[0].plot(x[mask], y[mask], '+', c='lightgrey', ms=8)
-    ax[0].plot(x[~mask], y[~mask], '+', c='black', ms=8)
+    ax[0].plot(x[~m], y[~m], '+', c='black', ms=8, zorder=-2)
+    ax[0].plot(x[m], y[m], '+', c='lightgrey', ms=8, zorder=-3)
+
+    # Settings
+    ax[0].set_xlim(x_fit[0], x_fit[-1])
+    ax[0].autoscale(False)
+
     # Fitted data
-    ax[0].plot(x_fit, y_fit, '-', c='red', lw=1.5)
+    ax[0].plot(x_fit, y_fit, '-', c='red', lw=1.5, zorder=-1)
     
     # Settings
     ax[0].grid(True, ls='--')
     # ticks
     ax[0].tick_params(
         which='major', direction='in', top=True, right=True, length=5, width=1.5, 
         labelsize=12)
     ax[0].minorticks_off()
-    # lim
-    ax[0].set_xlim(x_fit[0], x_fit[-1])
-    if ymin is not None:
-        if use_relative:
-            ax[0].set_ylim((y_fit.min() + y_fit.max() * ymin), y_fit.max() * (1 + ymax))
-        else:
-            ax[0].set_ylim(y_fit.min() + ymin, y_fit.max() + ymax)
     # labels
     ax[0].set_ylabel(ylabel, fontsize=16)
 
     # Residual
-    ax[1].plot(x[mask], residual[mask], '+', c='lightgrey', ms=8)
-    ax[1].plot(x[~mask], residual[~mask], '+', c='black', ms=8)
+    ax[1].plot(x[m], r[m], '+', c='lightgrey', ms=8)
+    ax[1].plot(x[~m], r[~m], '+', c='black', ms=8)
     ax[1].axhline(y=0, ls='-', c='red', lw=1.5)
     if threshold_lower is not None:
         ax[1].axhline(y=threshold_lower, ls='--', c='red', lw=1.5)
     if threshold_upper is not None:
         ax[1].axhline(y=threshold_upper, ls='--', c='red', lw=1.5)
     
     # Settings
@@ -80,17 +86,19 @@
     # label
     ax[1].set_xlabel(xlabel, fontsize=16)
     if use_relative:
         label_residual = 'rel. residual'
     else:
         label_residual = 'residual'
     ax[1].set_ylabel(label_residual, fontsize=16)
+    ax[1].annotate(
+        f'RMS$={rms:.3}$', (0.8, 0.8), xycoords='axes fraction', fontsize=12)
 
-    
-def plotFitting(x, y, residual, mask, y_fit, x_fit=None, threshold_lower=None, 
+
+def plotFitting(x, y, m, y_fit, r, x_fit=None, threshold_lower=None, 
                 threshold_upper=None, xlabel='x', ylabel='y', title='fitting', 
                 show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, 
                 use_relative=False):
     """Plot fitting.
 
     Parameters
     ----------
@@ -101,23 +109,22 @@
         Whether to save plot.
 
     path : bool, optional
         Path to save plot in.
     """
 
     _validateBool(show, 'show')
+    _validateBool(save, 'save')
 
-    _validateString(title, 'title')
-    if title != 'fitting':
-        title = f'{title} fitting'
+    if show | save:
 
-    fig_path = _validatePath(save, path, title)
+        _validateString(title, 'title')
+        if title != 'fitting':
+            title = f'{title} fitting'
 
-    if show | save:
-        
         if x_fit is None:
             x_fit = deepcopy(x)
 
         if threshold_lower is not None:
             if np.isnan(threshold_lower) | np.isinf(threshold_lower):
                 threshold_lower = None
             else:
@@ -131,24 +138,29 @@
                 _validateRange(
                     threshold_upper, 'threshold_upper', (0, None), (True, None))
 
         _validateBool(use_relative, 'use_relative')
 
         fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
         fig.subplots_adjust(hspace=0)
+
         _plotFitting(
-            ax, x, y, residual, mask, y_fit, x_fit, threshold_lower, threshold_upper, 
-            xlabel, ylabel, use_relative)
+            ax, x, y, m, x_fit, y_fit, r, threshold_lower, threshold_upper, xlabel, 
+            ylabel, use_relative)
+
         ax[0].set_title(title, fontsize=16)
         fig.align_ylabels()
         fig.tight_layout()
         
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
 
 def _plotSpectrum1D(ax, spectral_axis, flux, uncertainty=None, xlabel='spectral axis', 
                     ylabel='flux'):
     """Plot 1-dimensional spectrum of type `~specutils.Spectrum1D`."""
@@ -197,30 +209,25 @@
         Whether to save plot.
 
     path : bool, optional
         Path to save plot in.
     """
 
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-    if title != 'spectrum':
-        title = f'{title} spectrum'
-
-    fig_path = _validatePath(save, path, title)
+    _validateBool(save, 'save')
 
     if show | save:
 
+        _validateString(title, 'title')
+        if title != 'spectrum':
+            title = f'{title} spectrum'
+
         new_spectrum1d, spectral_axis, flux, uncertainty, mask = _validateSpectrum(
             spectrum1d, 'spectrum1d', True, True)
 
-        # Apply mask
-        flux[mask] = np.nan
-        uncertainty[mask] = np.nan
-
         # Labels
         unit_spectral_axis = new_spectrum1d.spectral_axis.unit.to_string()
         unit_flux = new_spectrum1d.flux.unit.to_string()
 
         xlabel = f'spectral axis [{unit_spectral_axis}]'
         ylabel = f'flux [{unit_flux}]'
 
@@ -228,17 +235,20 @@
         _plotSpectrum1D(
             ax, spectral_axis, flux, uncertainty, xlabel=xlabel, ylabel=ylabel)
         # ax.legend(fontsize=16)
         ax.set_title(title, fontsize=16)
         fig.set_figheight(0.7 * fig.get_figwidth())
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
 
 def _plot2d(ax, ccd, cmap='Greys_r', contrast=0.25, cbar=True, xlabel='column', 
             ylabel='row', cblabel='pixel value', **kwargs):
     """Plot image."""
@@ -275,15 +285,15 @@
         # Settings
         cb.ax.tick_params(
             which='major', direction='in', right=True, color='w', length=5, width=1.5, 
             labelsize=12)
         cb.ax.set_ylabel(cblabel, fontsize=16)
 
 
-def plot2d(ccd, cmap='Greys_r', contrast=0.25, extent=None, cbar=True, xlabel='column', 
+def plot2d(ccd, cmap='Greys_r', contrast=0.25, cbar=True, xlabel='column', 
            ylabel='row', cblabel='pixel value', title='image', show=conf.fig_show, 
            save=conf.fig_save, path=conf.fig_path, **kwargs):
     """Plot image.
 
     Parameters
     ----------
     show : bool, optional
@@ -293,30 +303,29 @@
         Whether to save plot.
 
     path : bool, optional
         Path to save plot in.
     """
 
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-
-    fig_path = _validatePath(save, path, title)
+    _validateBool(save, 'save')
 
     if show | save:
 
-        if extent is None:
-            extent = (-0.5, ccd.shape[1] - 0.5, -0.5, ccd.shape[0] - 0.5)
+        _validateString(title, 'title')
 
         fig, ax = plt.subplots(1, 1, dpi=100)
         _plot2d(
-            ax=ax, ccd=ccd, cmap=cmap, contrast=contrast, extent=extent, cbar=cbar, 
-            xlabel=xlabel, ylabel=ylabel, cblabel=cblabel, **kwargs)
+            ax=ax, ccd=ccd, cmap=cmap, contrast=contrast, cbar=cbar, xlabel=xlabel, 
+            ylabel=ylabel, cblabel=cblabel, **kwargs)
         ax.set_title(title, fontsize=16)
         fig.set_figheight(ccd.shape[0] / ccd.shape[1] * fig.get_figwidth())
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/twodspec/longslit.py` & `astro-drpy-0.0.1.7/src/drpy/twodspec/longslit.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,47 +8,52 @@
 from scipy.optimize import OptimizeWarning
 # matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 # AstroPy
 import astropy.units as u
 from astropy.time import Time
+from astropy.stats import sigma_clip
 from astropy.nddata import CCDData, StdDevUncertainty
 from astropy.convolution import convolve_fft, Gaussian2DKernel, interpolate_replace_nans
+from astropy.utils.exceptions import AstropyUserWarning
 # ccdproc
 from ccdproc import flat_correct
 # specutils
 from specutils import Spectrum1D
 # drpy
 from drpy import conf
 from drpy.batch import CCDDataList
 from drpy.onedspec import loadExtinctionCurve
 from drpy.onedspec.center import _center1D_Gaussian, _refinePeakBases, _refinePeaks
 from drpy.modeling import Poly1D, Spline1D, Spline2D, GaussianSmoothing2D
-from drpy.plotting import plotFitting, _plotFitting, plot2d, _plot2d, _plotSpectrum1D
+from drpy.plotting import plotFitting, _plotFitting, plot2d, _plot2d
 from drpy.validate import (_validateBool, _validateString, _validateRange, 
                            _validateInteger, _validate1DArray, _validateNDArray, 
                            _validateCCDData, _validateCCDList, _validateCCD, 
                            _validateSpectrum, _validateBins, _validateAperture, 
                            _validatePath)
+from drpy.decorate import ignoreWarning
 
 from .utils import invertCoordinateMap
 
+sigma_clip = ignoreWarning(sigma_clip, 'ignore', AstropyUserWarning)
+
 # Set plot parameters
 plt.rcParams['figure.figsize'] = [conf.fig_width, conf.fig_width]
 plt.rcParams['axes.linewidth'] = 1.5
 plt.rcParams['mathtext.fontset'] = 'stix'
 plt.rcParams['font.family'] = 'STIXGeneral'
 
 __all__ = ['response', 'illumination', 'align', 'fitcoords', 'transform', 'trace', 
-           'background', 'extract', 'calibrate2d']
+           'background', 'profile', 'extract', 'calibrate2d']
 
 
-def response(ccd, slit_along, n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, 
-             grow=False, use_mask=False, show=conf.fig_show, save=conf.fig_save, 
+def response(ccd, slit_along, n_piece=3, maxiters=5, sigma_lower=None, 
+             sigma_upper=None, grow=False, use_mask=False, plot=True, 
              path=conf.fig_path):
     """Determine response calibration.
 
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
@@ -58,16 +63,18 @@
         calculations. Note that this will NOT affect the returned frame, which is 
         always of the same shape as ``ccd``.
 
     n_piece : int, optional
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is `3`.
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`.
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -105,45 +112,39 @@
     data_arr[mask_arr] = np.nan
 
     # Average along spatial (slit) axis
     x = np.arange(n_col)
     # Bad pixels (NaNs or infs) in the original frame (if any) may lead to unmasked 
     # elements in ``y`` and may cause an error in the spline fitting below.
     y = np.nanmean(data_arr, axis=0)
-    mask_y = np.all(mask_arr, axis=0)
+    m_y = np.all(mask_arr, axis=0)
 
     # Fit cubic spline function (always float64)
     spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
-        x=x, y=y, weight=None, mask=mask_y, order=3, n_piece=n_piece, n_iter=n_iter, 
+        x=x, y=y, m=m_y, order=3, n_piece=n_piece, maxiters=maxiters,  
         sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, use_relative=True)
     
     # Control precision
     y_fit = spl(x).astype(ccd.dtype)
-    rms_y_fit = (y_fit * residual)[~master_mask].std(dtype=ccd.dtype)
 
     # Fitting plot
     plotFitting(
-        x=x, y=y, residual=residual, mask=master_mask, x_fit=x, y_fit=y_fit, 
+        x=x, y=y, m=master_mask, y_fit=y_fit, r=residual, 
         threshold_lower=threshold_lower, threshold_upper=threshold_upper, 
         xlabel='dispersion axis [px]', ylabel='pixel value', title='response', 
-        show=show, save=save, path=path, use_relative=True)
+        show=False, save=plot, path=path, use_relative=True)
 
     if slit_along == 'col':
         rccd = CCDData(
-            data=(np.tile(y_fit, (n_row, 1)) * nccd.unit), 
-            uncertainty=StdDevUncertainty(np.full((n_row, n_col), rms_y_fit)), 
-            mask=np.tile(master_mask, (n_row, 1))
-        )
-
+            data=(np.tile(y_fit, (n_row, 1)) * nccd.unit), uncertainty=None, 
+            mask=np.tile(master_mask, (n_row, 1)))
     else:
         rccd = CCDData(
-            data=(np.tile(y_fit, (n_row, 1)).T * nccd.unit), 
-            uncertainty=StdDevUncertainty(np.full((n_col, n_row), rms_y_fit)), 
-            mask=np.tile(master_mask, (n_row, 1)).T
-        )
+            data=(np.tile(y_fit, (n_row, 1)).T * nccd.unit), uncertainty=None, 
+            mask=np.tile(master_mask, (n_row, 1)).T)
 
     # Response calibrated frame
     nccd = flat_correct(ccd=nccd, flat=rccd, norm_value=1)
 
     if ccd.uncertainty is None:
         nccd.uncertainty = None
 
@@ -155,23 +156,24 @@
         nccd.header['RESPONSE'] = '{} Response corrected.'.format(
             Time.now().to_value('iso', subfmt='date_hm'))
 
     elif np.ma.isMaskedArray(ccd):
         nccd = np.ma.array(nccd.data, mask=nccd.mask)
 
     else:
-        nccd = deepcopy(nccd.data)
+        nccd = nccd.data.copy()
 
     return nccd
 
 # todo: doc.
-def illumination(ccd, slit_along, method, sigma=None, n_piece=None, bins=5, n_iter=5, 
+def illumination(ccd, slit_along, method, sigma=None, n_piece=None, bins=5, maxiters=5, 
                  sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
-                 show=conf.fig_show, save=conf.fig_save, path=conf.fig_path):
-    """Model illumination.
+                 plot=conf.fig_save, path=conf.fig_path):
+    """Model illumination. Uncertainty of the model may be dominated by systematic 
+    error which cannot be estimated from data.
 
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
 
     slit_along : str
@@ -197,16 +199,18 @@
     
     bins : int or sequence of scalars, optional
         If `int`, it defines the number of equal-width bins. If a sequence, it defines 
         a monotonically increasing array of bin edges, including the rightmost edge, 
         allowing for non-uniform bin widths.
         Default is `5`.
         
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`. 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -242,21 +246,19 @@
 
     n_row, n_col = data_arr.shape
     
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
     # The largest allowed value for bin edge is set to ``n_col`` (or ``n_row`` 
     # depending on ``slit_along``) in order to enable the access to the last column (or 
-    # row), i.e., data_arr[:, bin_edges[0][0]:bin_edges[0][1]].
+    # row), i.e., data_arr[:, bin_edges[-1][0]:bin_edges[-1][1]].
     if slit_along == 'col':
-        bin_edges = _validateBins(bins, n_col)
+        bin_edges, loc_bin, n_bin = _validateBins(bins, n_col)
     else:
-        bin_edges = _validateBins(bins, n_row)
-    n_bin = bin_edges.shape[0]
-    loc_bin = (bin_edges.sum(axis=1) - 1) / 2
+        bin_edges, loc_bin, n_bin = _validateBins(bins, n_row)
     
     _validateString(method, 'method', ['Gaussian2D', 'CubicSpline2D', 'iraf'])
 
     if '2D' in method: # 2-dimensional method (`Gaussian2D` or `CubicSpline2D`)
         
         if slit_along == 'col':
 
@@ -313,42 +315,39 @@
                 data_arr_extended, kernel, boundary='fill', fill_value=0., 
                 convolve=convolve_fft)[y_pad:-y_pad, x_pad:-x_pad]
 
         if method == 'Gaussian2D':
 
             data_fit, residual, threshold_lower, threshold_upper, master_mask = (
                 GaussianSmoothing2D(
-                    x=X, y=Y, z=data_arr, sigma=sigma, mask=None, n_iter=n_iter, 
-                    sigma_lower=sigma_lower, sigma_upper=sigma_upper, axis=0, 
-                    grow=grow, use_relative=True)
+                    X, Y, data_arr, sigma, maxiters=maxiters, sigma_lower=sigma_lower, 
+                    sigma_upper=sigma_upper, axis=0, grow=grow, use_relative=True)
             )
 
         elif method == 'CubicSpline2D':
             
             bispl, residual, threshold_lower, threshold_upper, master_mask = Spline2D(
-                x=X, y=Y, z=data_arr, weight=None, mask=None, order=(3, 3), 
-                n_piece=n_piece, n_iter=n_iter, sigma_lower=sigma_lower, 
-                sigma_upper=sigma_upper, axis=0, grow=grow, use_relative=True)
+                x=X, y=Y, z=data_arr, order=(3, 3), n_piece=n_piece, maxiters=maxiters, 
+                sigma_lower=sigma_lower, sigma_upper=sigma_upper, axis=0, grow=grow, 
+                use_relative=True)
 
             data_fit = bispl(idx_col, idx_row, grid=True).T
         
         master_mask |= mask_arr
         
         data_fit = data_fit.astype(ccd.dtype)
-        rms_arr = np.full(
-            (n_row, n_col), (data_fit * residual)[~master_mask].std(dtype=ccd.dtype))
 
         # In 2D case, ``loc_bin`` is only used as index, thus converted to ``int``.
         idx_bin = loc_bin.astype(int)
         bin_data_arr = data_arr[:, idx_bin].T
         bin_data_fit = data_fit[:, idx_bin].T
         bin_mask_arr = master_mask[:, idx_bin].T
         bin_residual = residual[:, idx_bin].T
         # Both are `None` originally
-        if n_iter == 0:
+        if maxiters == 0:
             bin_threshold_lower = [None] * n_bin
             bin_threshold_upper = [None] * n_bin
         # Both ``threshold_lower`` and ``threshold_upper`` are 2-dimensional arrays, 
         # though each array only has one row. Use flatten to get rid of the additional 
         # dimension.
         else:
             bin_threshold_lower = threshold_lower.flatten()[idx_bin]
@@ -357,15 +356,14 @@
     elif method == 'iraf':  # 1-dimensional method (`iraf`)
 
         n_piece = _validate1DArray(n_piece, 'n_piece', n_bin, True)
 
         # Apply mask
         data_arr[mask_arr] = np.nan
 
-        rms_arr = np.zeros_like(data_arr)
         master_mask = np.zeros_like(data_arr, dtype=bool)
 
         bin_data_arr = np.zeros((n_bin, n_row))
         bin_data_fit = np.zeros((n_bin, n_row))
         bin_mask_arr = np.zeros((n_bin, n_row), dtype=bool)
         bin_residual = np.zeros((n_bin, n_row))
         bin_threshold_lower = [None] * n_bin
@@ -376,89 +374,80 @@
             # spline fitting below.
             bin_data_arr[i] = np.nanmean(data_arr[:, bin_start:bin_end], axis=1)
             bin_mask = np.all(mask_arr[:, bin_start:bin_end], axis=1)
 
             # Fit cubic spline function
             bin_spl, bin_residual[i], bin_threshold_lower[i], bin_threshold_upper[i], \
             bin_mask_arr[i] = Spline1D(
-                x=idx_row, y=bin_data_arr[i], weight=None, mask=bin_mask, order=3, 
-                n_piece=n_piece[i], n_iter=n_iter, sigma_lower=sigma_lower, 
-                sigma_upper=sigma_upper, grow=grow, use_relative=True)
+                x=idx_row, y=bin_data_arr[i], m=bin_mask, order=3, n_piece=n_piece[i], 
+                maxiters=maxiters, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+                grow=grow, use_relative=True)
             bin_data_fit[i] = bin_spl(idx_row)
-            rms_arr[:, bin_start:bin_end] = (
-                bin_data_fit[i] * bin_residual[i])[~bin_mask_arr[i]].std()
             master_mask[bin_mask_arr[i], bin_start:bin_end] = True
         
         # Interpolate
         data_fit = interpolate.interp1d(
             x=loc_bin, y=bin_data_fit.T, axis=1, kind='linear', bounds_error=False, 
             fill_value='extrapolate', assume_sorted=True)(idx_col).astype(ccd.dtype)
 
     if slit_along != 'col':
         data_fit = data_fit.T
-        rms_arr = rms_arr.T
         master_mask = master_mask.T
         n_col, n_row = n_row, n_col
         idx_col, idx_row = idx_row, idx_col
 
     # Fitting plot
-    if slit_along == 'col':
-        x = idx_row
-    else:
-        x = idx_col
-    
-    _validateBool(show, 'show')
+    _validateBool(plot, 'plot')
 
-    fig_path = _validatePath(save, path, 'illumination fitting', '.pdf')
+    if plot:
 
-    if show | save:
+        if slit_along == 'col':
+            x = idx_row
+        else:
+            x = idx_col
 
+        fig_path = _validatePath(path, 'illumination fitting', '.pdf')
         with PdfPages(fig_path, keep_empty=False) as pdf:
 
             for i in range(n_bin):
 
                 fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
                 fig.subplots_adjust(hspace=0)
 
                 _plotFitting(
-                    ax=ax, x=x, y=bin_data_arr[i], residual=bin_residual[i], 
-                    mask=bin_mask_arr[i], x_fit=x, y_fit=bin_data_fit[i], 
+                    ax=ax, x=x, y=bin_data_arr[i], m=bin_mask_arr[i], x_fit=x, 
+                    y_fit=bin_data_fit[i], r=bin_residual[i], 
                     threshold_lower=bin_threshold_lower[i], 
                     threshold_upper=bin_threshold_upper[i], xlabel='spatial axis [px]', 
                     ylabel='pixel value', use_relative=True)
 
-                ax[0].set_title(f'profile at bin {loc_bin[i]}', fontsize=16)
+                ax[0].set_title(f'profile at column {loc_bin[i]}', fontsize=16)
                 fig.align_ylabels()
                 fig.tight_layout()
 
-                if save: pdf.savefig(fig, dpi=100)
-
-                if show: plt.show()
+                pdf.savefig(fig, dpi=100)
 
                 plt.close()
     
     # Illumination
-    nccd.data = deepcopy(data_fit)
-
-    if nccd.uncertainty is not None:
-        nccd.uncertainty.array = deepcopy(rms_arr)
-
+    nccd.data = data_fit.copy()
+    nccd.uncertainty = None
     if nccd.mask is not None:
         nccd.mask[master_mask] = True
 
     # Output
     if isinstance(ccd, CCDData):
         nccd.header['MKILLUM'] = '{} Illumination.'.format(
             Time.now().to_value('iso', subfmt='date_hm'))
 
     elif np.ma.isMaskedArray(ccd):
         nccd = np.ma.array(nccd.data, mask=nccd.mask)
 
     else:
-        nccd = deepcopy(nccd.data)
+        nccd = nccd.data.copy()
 
     return nccd
 
 
 def align(ccdlist, slit_along, index=0):
     """Align multiple frames.
     
@@ -545,17 +534,17 @@
             Time.now().to_value('iso', subfmt='date_hm'), shift)
         
         nccdlist.append(nccd)
 
     return CCDDataList(nccdlist)
 
 
-def fitcoords(ccd, slit_along, order=0, n_med=5, prominence=1e-3, n_piece=3, n_iter=5, 
-              sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
-              show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, **kwargs):
+def fitcoords(ccd, slit_along, order=0, n_med=5, prominence=1e-3, n_piece=3, 
+              maxiters=5, sigma_lower=None, sigma_upper=None, grow=False, 
+              use_mask=False, plot=conf.fig_save, path=conf.fig_path, **kwargs):
     """Fit distortion across the slit.
     
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `numpy.ndarray`
         Input frame.
     
@@ -575,16 +564,18 @@
     prominence ：scalar or `~numpy.ndarray` or sequence, optional
         Required prominence of peaks. see `~scipy.signal.find_peak` for details.
 
     n_piece : int, optional
         Number of spline pieces. Lengths are all equal. Must be positive.
         Default is `3`.
 
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`. 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -618,45 +609,44 @@
 
     n_row, n_col = data_arr.shape
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
     # Apply mask
     data_arr[mask_arr] = np.nan
-
-    _validateInteger(n_med, 'n_med', (1, None), (True, None))
     
     # Split into bins along spatial (slit) axis
-    bin_edges = np.hstack([np.arange(0, n_row, n_med), n_row])
-    bin_edges = np.vstack([bin_edges[:-1], bin_edges[1:]]).T
-    n_bin = bin_edges.shape[0]
-    loc_bin = (bin_edges.sum(axis=1) - 1) / 2
+    _validateInteger(n_med, 'n_med', (1, None), (True, None))
+    bin_edges, loc_bin, n_bin = _validateBins(n_med, n_row, isWidth=True)
+
+    idx_bin = np.arange(n_bin)
 
     bin_data_arr = np.zeros((n_bin, n_col))
 
     # A precision of 0.05 px for cross-correlation (can be changed)
     n_sub = 20
     # Of type `~numpy.float64`, although still named as an index array.
     idx_col_dense = np.linspace(0, idx_col[-1], idx_col[-1] * n_sub + 1)
     bin_data_arr_dense = np.zeros((n_bin, idx_col_dense.shape[0]))
 
     for i, (bin_start, bin_end) in enumerate(bin_edges):
+
         # Bad pixels should be labeled by ``mask_arr`` in advance
         bin_data = np.nanmean(data_arr[bin_start:bin_end, :], axis=0)
         bin_mask = np.all(mask_arr[bin_start:bin_end, :], axis=0)
 
         # Interpolate masked pixels to ensure finite results in cross-correlation
         fill_value = (bin_data[~bin_mask][0], bin_data[~bin_mask][-1])
         bin_data = interpolate.interp1d(
             x=idx_col[~bin_mask], y=bin_data[~bin_mask], bounds_error=False, 
             fill_value=fill_value, assume_sorted=True)(idx_col)
 
         # Normalize
         bin_data_arr[i] = bin_data / bin_data.max()
-        
+
         # Interpolate to a denser grid
         bin_data_arr_dense[i] = interpolate.interp1d(
             x=idx_col, y=bin_data_arr[i], assume_sorted=True)(idx_col_dense)
 
     # Reference spectrum
     idx_ref = n_bin // 2
     bin_data_ref_dense = bin_data_arr_dense[idx_ref]
@@ -669,47 +659,47 @@
     bin_data_ref_dense_ext = np.hstack(
         [bin_data_ref_dense[-n_ext * n_sub:], bin_data_ref_dense, 
          bin_data_ref_dense[:n_ext * n_sub]]
     )
 
     shift_arr = np.zeros(n_bin)
 
-    for i in range(n_bin):
+    for i in idx_bin:
         # Get zeropoint shift through cross-correlation
         idx_max = signal.correlate(
             bin_data_ref_dense_ext, bin_data_arr_dense[i], mode='valid', method='auto'
         ).argmax()
         shift_arr[i] = idx_ref_dense_ext[idx_max]
 
     _validateInteger(order, 'order', (0, 2), (True, True))
 
     if order == 0:
 
         # Univariate cubic spline fitting
         spl, residual, threshold_lower, threshold_upper, mask = Spline1D(
-            x=loc_bin, y=shift_arr, weight=None, mask=None, order=3, n_piece=n_piece, 
-            n_iter=n_iter, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
+            x=loc_bin, y=shift_arr, order=3, n_piece=n_piece, maxiters=maxiters, 
+            sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
         shift_fit = spl(idx_row)
 
         U = idx_col + shift_fit[:, np.newaxis]
 
         # Fitting plot
         plotFitting(
-            x=loc_bin, y=shift_arr, residual=residual, mask=mask, x_fit=idx_row, 
-            y_fit=shift_fit, threshold_lower=threshold_lower, 
-            threshold_upper=threshold_upper, xlabel='spatial axis [px]', 
-            ylabel='shift value [px]', title='zeropoint shift curve', show=show, 
-            save=save, path=path, use_relative=False)
+            x=loc_bin, y=shift_arr, m=mask, x_fit=idx_row, y_fit=shift_fit, r=residual, 
+            threshold_lower=threshold_lower, threshold_upper=threshold_upper, 
+            xlabel='spatial axis [px]', ylabel='shift value [px]', 
+            title='zeropoint shift curve', show=False, save=plot, path=path, 
+            use_relative=False)
 
     else:
 
         shift = np.round(shift_arr * n_sub).astype(int)
         rolled_bin_data_arr_dense = np.zeros_like(bin_data_arr_dense)
-        for i in range(n_bin):
+        for i in idx_bin:
             # Roll to align with reference spectrum
             rolled_bin_data_arr_dense[i] = np.roll(bin_data_arr_dense[i], shift[i])
         bin_data_mean = rolled_bin_data_arr_dense.mean(axis=0)[::n_sub]
 
         shift_max, shift_min = shift_arr.max(), shift_arr.min()
 
         if shift_max <= 0:
@@ -751,30 +741,30 @@
         peaks = refined_peaks + idx_start
         heights = heights[refined_index]
         left_bases = refined_left_bases[refined_index] + idx_start
         right_bases = refined_right_bases[refined_index] + idx_start
 
         refined_peaks_arr = np.full((n_bin, n_peak), np.nan)
 
-        for i in range(n_bin):
+        for i in idx_bin:
 
             # Offset peak properties
             shifted_peaks = peaks - shift_arr[i]
             shifted_left_bases = left_bases - shift_arr[i]
             shifted_right_bases = right_bases - shift_arr[i]
 
             # Refine peaks
             refined_peaks, refined_index = _refinePeaks(
                 bin_data_arr[i], shifted_peaks, heights, shifted_left_bases, 
                 shifted_right_bases, 1)
 
             refined_peaks_arr[i, refined_index] = refined_peaks
 
         # Fitcoords
-        x = deepcopy(refined_peaks_arr)
+        x = refined_peaks_arr.copy()
         y = np.tile(loc_bin, (n_peak, 1)).T
         z = np.tile(peaks, (n_bin, 1))
         mask = np.isnan(x) | np.isnan(z)
         # All the elements of ``x`` and ``y`` are within [idx_col[0], idx_col[-1]] and 
         # [idx_row[0], idx_row[-1]], respectively. Therefore, extrapolation is 
         # inevitably used when calculating z(x, y), which is defined on the whole 
         # frame. However, `~scipy.interpolate.LSQBivariateSpline` called by `Spline2D` 
@@ -782,113 +772,105 @@
         # we set ``bbox`` to be the boundary of the whole frame and therefore will get 
         # correct return when calling `~scipy.interpolate.LSQBivariateSpline.__call__`. 
         # Note that doing this will not change the fitting result as long as the 
         # internal knots remain the same. (Also see cautions mentioned by 
         # https://stackoverflow.com/questions/45904929.)
         bbox = [idx_col[0], idx_col[-1], idx_row[0], idx_row[-1]]
         bispl, residual, threshold_lower, threshold_upper, master_mask = Spline2D(
-            x=x, y=y, z=z, weight=None, mask=mask, order=(order, 3), 
-            n_piece=(1, n_piece), bbox=bbox, n_iter=n_iter, sigma_lower=sigma_lower, 
-            sigma_upper=sigma_upper, axis=None, grow=grow, use_relative=False)
+            x=x, y=y, z=z, m=mask, order=(order, 3), n_piece=(1, n_piece), bbox=bbox, 
+            maxiters=maxiters, sigma_lower=sigma_lower, sigma_upper=sigma_upper, axis=None, 
+            grow=grow, use_relative=False)
 
         # !!! Extrapolation is used here (see above) !!!
         U = bispl(idx_col, idx_row, grid=True).T
 
         # Plot
-        _validateBool(show, 'show')
-
-        title = 'peak detection'
+        _validateBool(plot, 'plot')
 
-        fig_path = _validatePath(save, path, title)
-        fig_path_fitting = _validatePath(save, path, 'distortion fitting', '.pdf')
-
-        if show | save:
+        if plot:
+            
+            # Peak detection plot
+            title = 'peak detection'
             
-            # Peak detection
-            fig = plt.figure(dpi=100)
             # Split into subplots
             n_subplot = 2
+
+            fig, ax = plt.subplots(n_subplot, 1, dpi=100)
+
             length = n_col // n_subplot + 1
             for i in range(n_subplot):
+
                 idx_start, idx_end = i * length, (i + 1) * length
                 idx_peak = np.where((idx_start <= peaks) & (peaks < idx_end))[0]
-                ax = fig.add_subplot(n_subplot, 1, i + 1)
-                ax.step(
+
+                ax[i].step(
                     idx_col[idx_start:idx_end], bin_data_mean[idx_start:idx_end], 
                     color='k', ls='-', where='mid')
                 for idx in idx_peak:
                     ymin = heights[idx] * 1.2
                     ymax = heights[idx] * 1.5
-                    ax.plot([peaks[idx], peaks[idx]], [ymin, ymax], 'r-', lw=1.5)
+                    ax[i].plot([peaks[idx], peaks[idx]], [ymin, ymax], 'r-', lw=1.5)
+
                 # Settings
-                ax.grid(axis='both', color='0.95', zorder=-1)
-                ax.set_xlim(idx_start, idx_end)
-                ax.set_yscale('log')
-                ax.tick_params(
+                ax[i].grid(axis='both', color='0.95', zorder=-1)
+                ax[i].set_xlim(idx_start, idx_end)
+                ax[i].set_yscale('log')
+                ax[i].tick_params(
                     which='major', direction='in', top=True, right=True, length=5, 
                     width=1.5, labelsize=12)
-                ax.tick_params(
+                ax[i].tick_params(
                     which='minor', direction='in', top=True, right=True, length=3, 
                     width=1.5, labelsize=12)
-                ax.set_ylabel('normalized intensity', fontsize=16)
-            ax.set_xlabel('dispersion axis [px]', fontsize=16)
-            ax.set_title(title, fontsize=16)
+                ax[i].set_ylabel('normalized intensity', fontsize=16)
+            ax[-1].set_xlabel('dispersion axis [px]', fontsize=16)
+            ax[0].set_title(title, fontsize=16)
             fig.align_ylabels()
+            fig.set_figheight(fig.get_figwidth() * n_subplot / 2)
             fig.tight_layout()
 
-            if save: plt.savefig(fig_path, dpi=100)
+            # Save
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-            if show: plt.show()
-            
             plt.close()
 
-            # Distortion fitting
-            if n_bin // 10 >= 10:
-                idx_plot = np.linspace(0, n_bin - 1, 11).astype(int)
-
-            else:
-                idx_plot = np.arange(0, n_bin, 10)
-                if idx_plot[-1] != n_bin - 1:
-                    idx_plot = np.hstack([idx_plot, n_bin - 1])
-
+            # Distortion fitting plot
             z_fit = bispl(idx_col, loc_bin, grid=True).T
-            
-            with PdfPages(fig_path_fitting, keep_empty=False) as pdf:
 
-                for i in idx_plot:
+            fig_path = _validatePath(path, 'distortion fitting', '.pdf')
+            with PdfPages(fig_path, keep_empty=False) as pdf:
+
+                for i in idx_bin[::10]:
 
                     fig, ax = plt.subplots(
                         2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
                     fig.subplots_adjust(hspace=0)
 
                     _plotFitting(
                         ax=ax, x=refined_peaks_arr[i], 
-                        y=(peaks - refined_peaks_arr[i]), residual=residual[i], 
-                        mask=master_mask[i], x_fit=idx_col, y_fit=(z_fit[i] - idx_col), 
+                        y=(peaks - refined_peaks_arr[i]), m=master_mask[i], 
+                        x_fit=idx_col, y_fit=(z_fit[i] - idx_col), r=residual[i], 
                         threshold_lower=threshold_lower, 
                         threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
                         ylabel='shift [px]', use_relative=False)
 
                     ax[0].set_title(f'distortion at bin {loc_bin[i]}', fontsize=16)
                     fig.align_ylabels()
                     fig.tight_layout()
 
-                    if save: pdf.savefig(fig, dpi=100)
-
-                    if show: plt.show()
+                    pdf.savefig(fig, dpi=100)
 
                     plt.close()
 
-        # Distortion residual
+        # Distortion residual image
         residual[master_mask] = np.nan
         cmap = plt.cm.get_cmap('Greys_r').copy(); cmap.set_bad('red', 1.)
-        extent = (-0.5, residual.shape[1] - 0.5, -0.5, residual.shape[0] - 0.5)
         plot2d(
             residual, cmap=cmap, xlabel='peak number', ylabel='bin number', 
-            cblabel='pixel', title='distortion residual', show=show, save=save, 
+            cblabel='pixel', title='distortion residual', show=False, save=plot, 
             path=path)
 
     V = np.tile(idx_row, (n_col, 1)).T
 
     # Output
     if slit_along != 'col':
         U, V = V.T, U.T
@@ -914,17 +896,15 @@
     
     Returns
     -------
     nccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         The transformed frame.
     """
 
-    nccd = _validateCCDData(ccd, 'ccd')
-
-    data_arr = deepcopy(nccd.data)
+    nccd, data_arr, _, _ = _validateCCD(ccd, 'ccd', False, False, False)
 
     n_row, n_col = data_arr.shape
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
     _validateNDArray(X, 'X', 2)
     _validateNDArray(Y, 'Y', 2)
@@ -953,57 +933,57 @@
     else:
         S = 1.
 
     # Data
     data_arr_transformed = ndimage.map_coordinates(
         input=data_arr, coordinates=(Y, X), order=1, mode='nearest')
     data_arr_transformed *= S
-    nccd.data = deepcopy(data_arr_transformed)
+    nccd.data = data_arr_transformed.copy()
 
     # Uncertainty
     # This method is simple but enlarges the resulting uncertainty.
     if nccd.uncertainty is not None:
-        uncertainty_arr = deepcopy(nccd.uncertainty.array)
+        uncertainty_arr = nccd.uncertainty.array.copy()
         uncertainty_arr_transformed = np.sqrt(
             ndimage.map_coordinates(
                 input=uncertainty_arr**2, coordinates=(Y, X), order=1, mode='nearest')
         )
         uncertainty_arr_transformed *= S
-        nccd.uncertainty.array = deepcopy(uncertainty_arr_transformed)
+        nccd.uncertainty.array = uncertainty_arr_transformed.copy()
 
     # Mask
     if nccd.mask is not None:
         mask_arr = nccd.mask.astype(float)
         mask_arr_transformed = ndimage.map_coordinates(
             input=mask_arr, coordinates=(Y, X), order=1, mode='constant', cval=1.)
         # Any interpolated value of 0.1 or greater is given the value 1 in the output 
         # mask. The choice of 0.1 is purely empirical and gives an approximate 
         # identification of significant affected pixels. (for details see 
         # https://iraf.net/irafhelp.php?val=longslit.transform&help=Help+Page)
         threshold = 0.1
         mask_arr_transformed[mask_arr_transformed >= threshold] = 1.
         mask_arr_transformed = np.round(mask_arr_transformed).astype(bool)
-        nccd.mask = deepcopy(mask_arr_transformed)
+        nccd.mask = mask_arr_transformed.copy()
 
     # Output
     if isinstance(ccd, CCDData):
         nccd.header['TRANSFOR'] = '{} Transformed.'.format(
             Time.now().to_value('iso', subfmt='date_hm'))
 
     elif np.ma.isMaskedArray(ccd):
         nccd = np.ma.array(nccd.data, mask=nccd.mask)
 
     else:
-        nccd = deepcopy(nccd.data)
+        nccd = nccd.data.copy()
 
     return nccd
 
 # todo: doc
 def trace(ccd, slit_along, fwhm, method, n_med=3, reference_bin=None, interval=None, 
-          n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, grow=False, 
+          n_piece=3, maxiters=5, sigma_lower=None, sigma_upper=None, grow=False, 
           use_mask=False, title='trace', show=conf.fig_show, save=conf.fig_save, 
           path=conf.fig_path):
     """Trace on the 2-dimensional spectrum.
     
     First the spatial profiles are binned by taking median along the dispersion axis. 
     Then the center of the specified feature (that is the strongest one in the 
     interval) in the reference bin is determined by fitting a Gaussian profile. [...]
@@ -1043,16 +1023,18 @@
         - if 2-tuple, the brightest source in the interval is traced. (Use this when 
         the source is not the brightest one in the frame)
     
     n_piece : int, optional
         Number of spline pieces. Lengths are all equal. Must be positive. 
         Default is `3`.
     
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`. 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
@@ -1083,23 +1065,17 @@
     else:
         nccd, data_arr, _, mask_arr = _validateCCD(ccd, 'ccd', False, use_mask, True)
 
     n_row, n_col = data_arr.shape
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
     
-    _validateInteger(n_med, 'n_med', (3, None), (True, None))
-    
     # Split into bins along dispersion axis
-    bin_edges = np.arange(0, n_col, n_med)
-    if bin_edges[-1] < (n_col - 1):
-        bin_edges = np.hstack([bin_edges, (n_col - 1)])
-    bin_edges = np.vstack([bin_edges[:-1], bin_edges[1:]]).T
-    n_bin = bin_edges.shape[0]
-    loc_bin = (bin_edges.sum(axis=1) - 1) / 2
+    _validateInteger(n_med, 'n_med', (3, None), (True, None))
+    bin_edges, loc_bin, n_bin = _validateBins(n_med, n_col, isWidth=True)
     
     # If `None`, the reference bin will be the middle bin when the total number is odd 
     # while the first bin of the second half when the total number is even.
     if reference_bin is not None:
         _validateInteger(reference_bin, 'reference_bin', (0, (n_bin - 1)), (True, True))
     else:
         reference_bin = n_bin // 2
@@ -1134,38 +1110,38 @@
     # Normalize
     y_ref = count_ref[idx_min_ref:(idx_max_ref + 1)] / count_ref[idx_src_ref]
     m_ref = mask_ref[idx_min_ref:(idx_max_ref + 1)]
     
     # Gaussian fitting
     try:
         center_ref = _center1D_Gaussian(x_ref[~m_ref], y_ref[~m_ref], initial_guess, 0)
-        
+    
     except (RuntimeError, TypeError, OptimizeWarning): # raise exception here
         raise RuntimeError('No trace found in the given interval.')
     
     _validateString(method, 'method', ['center', 'trace'])
-
+    
     if method == 'center':
-
+    
         fitted_trace = np.full(n_col, center_ref)
-        
+    
     else:
         
         refined_trace = np.full(n_bin, np.nan)
         refined_trace[reference_bin] = center_ref
-        
+
         for i in range(reference_bin + 1, n_bin):
 
             # Bad pixels (NaNs or infs) in the original frame (if any) may lead to 
             # unmasked elements in ``count_bin`` and may cause an error in the 
             # Gaussian fitting below.
             count_bin = np.nanmedian(
                 data_arr[:, bin_edges[i][0]:bin_edges[i][1]], axis=1)
             mask_bin = np.all(mask_arr[:, bin_edges[i][0]:bin_edges[i][1]], axis=1)
-            
+
             # Peak range
             idx_ref = np.where(~np.isnan(refined_trace))[0].max()
             idx_min_bin = int(refined_trace[idx_ref] - 0.5 * fwhm)
             idx_max_bin = int(refined_trace[idx_ref] + 0.5 * fwhm)
 
             # Peak center
             idx_src_bin = idx_min_bin + np.ma.argmax(
@@ -1223,517 +1199,846 @@
             except (RuntimeError, TypeError, OptimizeWarning): # raise exception here
                 continue
 
         mask = np.isnan(refined_trace)
         
         # Spline fitting
         spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
-            x=loc_bin, y=refined_trace, weight=None, mask=mask, order=3, n_piece=n_piece, 
-            n_iter=n_iter, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
+            x=loc_bin, y=refined_trace, m=mask, order=3, n_piece=n_piece, 
+            maxiters=maxiters, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
 
         fitted_trace = spl(idx_col)
     
-    # Trace plot
+    # Plot
     _validateBool(show, 'show')
+    _validateBool(save, 'save')
 
-    _validateString(title, 'title')
-    if title != 'trace':
-        title = f'{title} trace'
+    if show | save:
 
-    fig_path = _validatePath(save, path, title)
+        _validateString(title, 'title')
+        if title != 'trace':
+            title = f'{title} trace'
 
-    if show | save:
-        
+        # Trace fitting plot
         if method == 'trace':
             plotFitting(
-                x=loc_bin, y=refined_trace, residual=residual, mask=master_mask, 
-                x_fit=idx_col, y_fit=fitted_trace, threshold_lower=threshold_lower, 
+                x=loc_bin, y=refined_trace, m=master_mask, x_fit=idx_col, 
+                y_fit=fitted_trace, r=residual, threshold_lower=threshold_lower, 
                 threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
                 ylabel='spatial axis [px]', title=title, show=show, save=save, 
                 path=path, use_relative=False)
 
+        # Trace image
         if slit_along == 'col':
             height_ratios = (1 / 4.5, n_col / n_row)
-            extent = (-0.5, n_row - 0.5, 0.5, n_col - 0.5)
         else:
-            extent = (-0.5, n_col - 0.5, 0.5, n_row - 0.5)
             height_ratios = (1 / 4.5, n_row / n_col)
         fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=height_ratios, dpi=100)
 
         # Subplot 1
         ax[0].step(idx_row, count_ref, 'k-', lw=1.5, where='mid')
-        ax[0].axvline(x=center_ref, color='r', ls='-', lw=1.5)
+        ax[0].axvline(x=center_ref, color='r', ls='--', lw=1.5)
 
         # Settings
         ax[0].grid(axis='both', color='0.95', zorder=-1)
         # ax[0].set_yscale('log')
         ax[0].tick_params(
             which='major', direction='in', top=True, right=True, length=5, width=1.5, 
             labelsize=12)
         ax[0].set_ylabel('pixel value', fontsize=16)
         ax[0].set_title(title, fontsize=16)
 
         # Subplot 2
         if slit_along == 'col':
             _plot2d(
-                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, extent=extent, 
-                cbar=False, xlabel='row', ylabel='column', aspect='auto')
+                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, cbar=False, 
+                xlabel='row', ylabel='column', aspect='auto')
         else:
             _plot2d(
-                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, extent=extent, 
-                cbar=False, aspect='auto')
+                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, cbar=False, 
+                aspect='auto')
         (xmin, xmax), (ymin, ymax) = ax[1].get_xlim(), ax[1].get_ylim()
-        ax[1].plot(fitted_trace, idx_col, 'r-', lw=1.5)
+        ax[1].plot(fitted_trace, idx_col, 'r--', lw=1.5)
 
         # Settings
         ax[1].set_xlim(xmin, xmax)
         ax[1].set_ylim(ymin, ymax)
         fig.set_figheight(fig.get_figwidth() * np.sum(height_ratios))
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
-    header = deepcopy(nccd.header)
+    header = nccd.header.copy()
     header['TRINTERV'] = f'{interval}'
     header['TRCENTER'] = center_ref
     header['TRACE'] = '{} Trace ({}, n_med = {}, n_piece = {})'.format(
         Time.now().to_value('iso', subfmt='date_hm'), method, n_med, n_piece)
     meta = {'header': header}
 
     # No uncertainty or mask frame
     trace1d = Spectrum1D(flux=(fitted_trace * u.pixel), meta=meta)
 
     return trace1d
 
 
-def background(ccd, slit_along, trace1d, distance=50, aper_width=50, degree=1, 
-               n_iter=5, sigma_lower=None, sigma_upper=None, grow=False, 
-               use_mask=False, title='background', show=conf.fig_show, 
-               save=conf.fig_save, path=conf.fig_path):
+def background(ccd, slit_along, trace1d, distance=75, aper_width=50, degree=0, 
+               maxiters=5, sigma_lower=None, sigma_upper=None, grow=False, 
+               use_uncertainty=False, use_mask=False, title='background', 
+               show=conf.fig_show, save=conf.fig_save, path=conf.fig_path):
     """Model background.
     
     Sky background of the input frame is modeled col by col (or row by row, depending 
     on the ``slit_along``) through polynomial fittings.
 
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
 
     slit_along : str
         `col` or `row`. If `row`, the data array of ``ccd`` will be transposed during 
         calculations. Note that this will NOT affect the returned frame, which is 
         always of the same shape as ``ccd``.
-    
+
     trace1d : `~specutils.Spectrum1D` or scalar or `~numpy.ndarray`
         Input trace.
-    
+
     distance : scalar or 2-tuple, optional
         Distances from the input trace to the centers of the two background apertures.
-    
+
     aper_width : scalar or 2-tuple, optional
         Aperture widths of the two background apertures.
-        
+
     degree : int, optional
         Degree of the fitting polynomial.
-        Default is `1`.
+        Default is `0`.
     
-    n_iter : int, optional
-        Number of sigma slipping iterations. Must be >= `0`. 
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
         Default is `5`.
 
     sigma_lower : scalar or `None`, optional
         Number of standard deviations to use as the lower bound for the clipping limit. 
         If `None` (default), `3` is used.
 
     sigma_upper : scalar or `None`, optional
         Number of standard deviations to use as the upper bound for the clipping limit. 
         If `None` (default), `3` is used.
     
     grow : scalar or `False`, optional
         Radius within which to mask the neighbouring pixels of those that fall outwith 
         the clipping limits.
 
+    use_uncertainty : bool, optional
+        If `True` and an uncertainty array is attributed to ``ccd``, the uncertainties 
+        are used as weights in the fitting. Note that weighted fitting is biased 
+        towards low values.
+        Default is `False`.
+
     use_mask : bool, optional
         If `True` and a mask array is attributed to ``ccd``, the masked pixels are 
         ignored in the fitting. 
         Default is `False`.
 
     Returns
     -------
     nccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Modeled background.
     """
 
     _validateString(slit_along, 'slit_along', ['col', 'row'])
 
+    _validateBool(use_uncertainty, 'use_uncertainty')
+
     _validateBool(use_mask, 'use_mask')
 
     if slit_along == 'col':
-        nccd, data_arr, _, mask_arr = _validateCCD(ccd, 'ccd', False, use_mask, False)
+        nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
+            ccd, 'ccd', use_uncertainty, use_mask, False, asWeight=True)
 
     else:
-        nccd, data_arr, _, mask_arr = _validateCCD(ccd, 'ccd', False, use_mask, True)
+        nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
+            ccd, 'ccd', use_uncertainty, use_mask, True, asWeight=True)
 
     n_row, n_col = data_arr.shape
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
-    # Assume that unit of the trace is [pixel]
+    # Weights (inverse variance weighted)
+    wght_arr = 1 / uncertainty_arr
+
+    # Assume that unit of the trace is [pixel]. No NaN is assumed.
     if isinstance(trace1d, Spectrum1D):
         trace1d = trace1d.flux.value
     trace1d = _validate1DArray(trace1d, 'trace1d', n_col, True)
 
     distance = _validate1DArray(distance, 'distance', 2, True)
 
     aper_width = _validate1DArray(aper_width, 'aper_width', 2, True)
     for i in range(2):
         _validateRange(aper_width[i], f'aper_width[{i}]', (1, None), (True, None))
 
     # Usually there are two separate background apertures (though they can be set 
     # overlapped). ``distance`` controls separations on either side of the trace.
-    idx_lbkg_min = trace1d - distance[0] - aper_width[0] / 2
-    idx_lbkg_max = trace1d - distance[0] + aper_width[0] / 2
-    idx_rbkg_min = trace1d + distance[1] - aper_width[1] / 2
-    idx_rbkg_max = trace1d + distance[1] + aper_width[1] / 2
-    
-    if (
-        (idx_lbkg_min.min() < -0.5) | (idx_lbkg_max.max() > (n_row - 0.5)) | 
-        (idx_rbkg_min.min() < -0.5) | (idx_rbkg_max.max() > (n_row - 0.5))
-    ):
+    idx_lbkgd_min = trace1d - distance[0] - aper_width[0] / 2
+    idx_lbkgd_max = trace1d - distance[0] + aper_width[0] / 2
+    idx_rbkgd_min = trace1d + distance[1] - aper_width[1] / 2
+    idx_rbkgd_max = trace1d + distance[1] + aper_width[1] / 2
+
+    idx_bkgd_min = np.vstack([idx_lbkgd_min, idx_rbkgd_min]).min()
+    idx_bkgd_max = np.vstack([idx_lbkgd_max, idx_rbkgd_max]).max()
+    if (idx_bkgd_min < -0.5) | (idx_bkgd_max > (n_row - 0.5)):
         warnings.warn('Background index out of range.', RuntimeWarning)
-    
-    bkg_arr = np.zeros_like(data_arr)
-    std_arr = np.zeros_like(data_arr)
 
     # Background fitting
+    bkgd_arr = np.zeros_like(data_arr)
+    rsdl_arr = np.zeros_like(data_arr) + np.nan
+    threshold_lower = [None] * n_col
+    threshold_upper = [None] * n_col
     for i in range(n_col):
 
-        mask_bkg = (
-            ((idx_lbkg_min[i] < idx_row) & (idx_row < idx_lbkg_max[i])) | 
-            ((idx_rbkg_min[i] < idx_row) & (idx_row < idx_rbkg_max[i]))
+        mask_bkgd = (
+            ((idx_lbkgd_min[i] < idx_row) & (idx_row < idx_lbkgd_max[i])) | 
+            ((idx_rbkgd_min[i] < idx_row) & (idx_row < idx_rbkgd_max[i]))
         )
 
-        p, residual, threshold_lower, threshold_upper, master_mask = Poly1D(
-            x=idx_row[mask_bkg], y=data_arr[mask_bkg, i], weight=None, 
-            mask=mask_arr[mask_bkg, i], degree=degree, n_iter=n_iter, 
+        p, rsdl_arr[mask_bkgd, i], threshold_lower[i], threshold_upper[i], \
+        mask_arr[mask_bkgd, i] = Poly1D(
+            x=idx_row[mask_bkgd], y=data_arr[mask_bkgd, i], w=wght_arr[mask_bkgd, i], 
+            m=mask_arr[mask_bkgd, i], deg=degree, maxiters=maxiters, 
             sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
 
-        bkg_arr[:, i] = p(idx_row)
-        mask_arr[mask_bkg, i][master_mask] = True
-        std_arr[:, i] = residual.std()
+        bkgd_arr[:, i] = p(idx_row)
 
+    # Plot
     _validateBool(show, 'show')
-
-    _validateString(title, 'title')
-    if title != 'background':
-        title = f'{title} background'
-
-    fig_path = _validatePath(save, path, title)
-    fig_path_fitting = _validatePath(save, path, f'{title} fitting', '.pdf')
+    _validateBool(save, 'save')
 
     if show | save:
 
+        _validateString(title, 'title')
+        if title != 'background':
+            title = f'{title} background'
+        
+        # Background image
         if slit_along == 'col':
             height_ratios = (1 / 4.5, n_col / n_row)
-            extent = (-0.5, n_row - 0.5, 0.5, n_col - 0.5)
         else:
-            extent = (-0.5, n_col - 0.5, 0.5, n_row - 0.5)
             height_ratios = (1 / 4.5, n_row / n_col)
         fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=height_ratios, dpi=100)
 
         # Subplot 1
         ax[0].step(idx_row, np.nanmedian(data_arr, axis=1), 'k-', lw=1.5, where='mid')
-        ax[0].axvline(x=idx_lbkg_min.mean(), color='y', ls='--', lw=1.5)
-        ax[0].axvline(x=idx_lbkg_max.mean(), color='y', ls='--', lw=1.5)
-        ax[0].axvline(x=idx_rbkg_min.mean(), color='b', ls='--', lw=1.5)
-        ax[0].axvline(x=idx_rbkg_max.mean(), color='b', ls='--', lw=1.5)
+        ax[0].axvline(x=idx_lbkgd_min.mean(), color='y', ls='--', lw=1.5)
+        ax[0].axvline(x=idx_lbkgd_max.mean(), color='y', ls='--', lw=1.5)
+        ax[0].axvline(x=idx_rbkgd_min.mean(), color='b', ls='--', lw=1.5)
+        ax[0].axvline(x=idx_rbkgd_max.mean(), color='b', ls='--', lw=1.5)
 
         # Settings
         ax[0].grid(axis='both', color='0.95', zorder=-1)
         ax[0].tick_params(
             which='major', direction='in', top=True, right=True, length=5, width=1.5, 
             labelsize=12)
         ax[0].set_ylabel('pixel value', fontsize=16)
         ax[0].set_title(title, fontsize=16)
 
         # Subplot 2
         if slit_along == 'col':
             _plot2d(
-                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, extent=extent, 
-                cbar=False, xlabel='row', ylabel='column', aspect='auto')
+                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, cbar=False, 
+                xlabel='row', ylabel='column', aspect='auto')
         else:
             _plot2d(
-                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, extent=extent, 
-                cbar=False, aspect='auto')
+                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, cbar=False, 
+                aspect='auto')
         (xmin, xmax), (ymin, ymax) = ax[1].get_xlim(), ax[1].get_ylim()
-        ax[1].plot(idx_lbkg_min, idx_col, 'y--', lw=1.5)
-        ax[1].plot(idx_lbkg_max, idx_col, 'y--', lw=1.5)
-        ax[1].plot(idx_rbkg_min, idx_col, 'b--', lw=1.5)
-        ax[1].plot(idx_rbkg_max, idx_col, 'b--', lw=1.5)
+        ax[1].plot(idx_lbkgd_min, idx_col, 'y--', lw=1.5)
+        ax[1].plot(idx_lbkgd_max, idx_col, 'y--', lw=1.5)
+        ax[1].plot(idx_rbkgd_min, idx_col, 'b--', lw=1.5)
+        ax[1].plot(idx_rbkgd_max, idx_col, 'b--', lw=1.5)
 
         # Settings
         ax[1].set_xlim(xmin, xmax)
         ax[1].set_ylim(ymin, ymax)
         fig.set_figheight(fig.get_figwidth() * np.sum(height_ratios))
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
-        # Background fitting plot
-        print(fig_path_fitting)
-        with PdfPages(fig_path_fitting, keep_empty=False) as pdf:
+    # Background fitting plot
+    if save:
+
+        idx_bkgd_range = idx_bkgd_max - idx_bkgd_min
+        mask_plot = (
+            ((idx_bkgd_min - 0.1 * idx_bkgd_range) <= idx_row) 
+            & (idx_row <= (idx_bkgd_max + 0.1 * idx_bkgd_range))
+        )
+
+        fig_path = _validatePath(path, f'{title} fitting', '.pdf')
+        with PdfPages(fig_path, keep_empty=False) as pdf:
 
             for i in idx_col[::10]:
 
                 fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
                 fig.subplots_adjust(hspace=0)
 
                 _plotFitting(
-                    ax=ax, x=idx_row, y=data_arr[:, i], 
-                    residual=(data_arr[:, i] - bkg_arr[:, i]), mask=mask_arr[:, i], 
-                    x_fit=idx_row, y_fit=bkg_arr[:, i], threshold_lower=None, 
-                    threshold_upper=None, xlabel='spatial axis [px]', 
+                    ax=ax, x=idx_row[mask_plot], y=data_arr[mask_plot, i], 
+                    m=mask_arr[mask_plot, i], x_fit=idx_row[mask_plot], 
+                    y_fit=bkgd_arr[mask_plot, i], r=rsdl_arr[mask_plot, i], 
+                    threshold_lower=threshold_lower[i], 
+                    threshold_upper=threshold_upper[i], xlabel='spatial axis [px]', 
                     ylabel='pixel value', use_relative=False)
 
+                ax[0].axvline(x=idx_lbkgd_min[i], color='y', ls='--', lw=1.5)
+                ax[0].axvline(x=idx_lbkgd_max[i], color='y', ls='--', lw=1.5)
+                ax[0].axvline(x=idx_rbkgd_min[i], color='b', ls='--', lw=1.5)
+                ax[0].axvline(x=idx_rbkgd_max[i], color='b', ls='--', lw=1.5)
+
+                # Settings
                 ax[0].set_title(f'background at column {i}', fontsize=16)
+
+                ax[1].axvline(x=idx_lbkgd_min[i], color='y', ls='--', lw=1.5)
+                ax[1].axvline(x=idx_lbkgd_max[i], color='y', ls='--', lw=1.5)
+                ax[1].axvline(x=idx_rbkgd_min[i], color='b', ls='--', lw=1.5)
+                ax[1].axvline(x=idx_rbkgd_max[i], color='b', ls='--', lw=1.5)
+
                 fig.align_ylabels()
                 fig.tight_layout()
 
-                if save: pdf.savefig(fig, dpi=100)
-
-                if show: plt.show()
+                pdf.savefig(fig, dpi=100)
 
                 plt.close()
 
     # Background frame
     if slit_along == 'col':
-        nccd.data = deepcopy(bkg_arr)
-
-        if nccd.uncertainty is not None:
-            nccd.uncertainty.array = deepcopy(std_arr)
 
+        nccd.data = bkgd_arr.copy()
+        nccd.uncertainty = None
         if nccd.mask is not None:
-            nccd.mask = deepcopy(mask_arr)
-    else:
-        nccd.data = bkg_arr.T
+            nccd.mask = mask_arr.copy()
 
-        if nccd.uncertainty is not None:
-            nccd.uncertainty.array = std_arr.T
+    else:
 
+        nccd.data = bkgd_arr.T
+        nccd.uncertainty = None
         if nccd.mask is not None:
             nccd.mask = mask_arr.T
 
     # Output
     if isinstance(ccd, CCDData):
         nccd.header['MKBACKGR'] = '{} Background.'.format(
             Time.now().to_value('iso', subfmt='date_hm'))
 
     elif np.ma.isMaskedArray(ccd):
         nccd = np.ma.array(nccd.data, mask=nccd.mask)
 
     else:
-        nccd = deepcopy(nccd.data)
+        nccd = nccd.data.copy()
 
     return nccd
 
 
-def extract(ccd, slit_along, trace1d, aper_width, method, psf_width=None, n_aper=1, 
-            spectral_axis=None, title='aperture', show=conf.fig_show, 
+def profile(ccd, slit_along, trace1d, profile_width, sigma, maxiters=5, 
+            sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
+            title='profile', show=conf.fig_show, save=conf.fig_save, 
+            path=conf.fig_path):
+    """Build an effective spatial profile along slit. Usually used by the optimal 
+    extraction algorithm.
+
+    Parameters
+    ----------
+    ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
+        Input frame. Should be background subtracted.
+
+    slit_along : str
+        `col` or `row`. If `row`, the data array of ``ccd`` will be transposed during 
+        calculations. Note that this will NOT affect the returned frame, which is 
+        always of the same shape as ``ccd``.
+
+    trace1d : `~specutils.Spectrum1D` or scalar or `~numpy.ndarray`
+        Input trace.
+
+    profile_width : scalar or 2-tuple
+        Profile width. Usually large widths are preferred. Pixels outside the profile 
+        will be set to `0`.
+    
+    sigma : scalar
+        Standard deviation for Gaussian filter.
+    
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
+        Default is `5`.
+
+    sigma_lower : scalar or `None`, optional
+        Number of standard deviations to use as the lower bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    sigma_upper : scalar or `None`, optional
+        Number of standard deviations to use as the upper bound for the clipping limit. 
+        If `None` (default), `3` is used.
+    
+    grow : scalar or `False`, optional
+        Radius within which to mask the neighbouring pixels of those that fall outwith 
+        the clipping limits.
+
+    use_mask : bool, optional
+        If `True` and a mask array is attributed to ``ccd``, the masked pixels are 
+        ignored in the fitting. 
+        Default is `False`.
+
+    Returns
+    -------
+    P_fit : `~numpy.ndarray`
+        Fitted spatial profile.
+    
+    nccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
+        The input frame with updated cosmic ray mask.
+    """
+
+    _validateString(slit_along, 'slit_along', ['col', 'row'])
+
+    _validateBool(use_mask, 'use_mask')
+
+    if slit_along == 'col':
+        nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
+            ccd, 'ccd', False, use_mask, transpose=False)
+    else:
+        nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
+            ccd, 'ccd', False, use_mask, transpose=True)
+
+    n_row, n_col = data_arr.shape
+
+    idx_row, idx_col = np.arange(n_row), np.arange(n_col)
+
+    # Assume that unit of the trace is [pixel]
+    if isinstance(trace1d, Spectrum1D):
+        try:
+            trcenter = trace1d.meta['header']['TRCENTER']
+        except:
+            trcenter = np.median(
+                _validate1DArray(trace1d.flux.value, 'trace1d', n_col, True)
+            )
+    else:
+        trcenter = np.median(_validate1DArray(trace1d, 'trace1d', n_col, True))
+
+    # The total profile width is the sum of the two elements in ``profile_width``. If 
+    # they have opposite signs, the whole aperture will be on the same side of the 
+    # trace.
+    profile_width = _validateAperture(profile_width, 'profile_width')
+    profile_width[0] *= -1; profile_width.sort()
+
+    profile_edges = np.round(trcenter + profile_width).astype(int)
+
+    n_frac = profile_edges[1] + 1 - profile_edges[0]
+
+    idx_frac = np.arange(n_frac)
+
+    slice_frac = slice(profile_edges[0], profile_edges[1] + 1)
+
+    # DS -- data with sky background subtracted (Horne 1986)
+    DS = data_arr.copy()
+
+    # V -- variance (Horne 1986)
+    V = uncertainty_arr**2
+
+    # f = Σ(D-S) --- object flux by summing along the spatial dimension (Horne 1986)
+    f = DS[slice_frac].sum(axis=0)
+
+    # Observed profile
+    P_obs = DS / f
+
+    # (X, Y) grid
+    X = np.tile(idx_col, (n_frac, 1))
+    Y = np.tile(idx_frac, (n_col, 1)).T
+
+    P_fit = np.zeros_like(P_obs)
+    master_mask = mask_arr.copy()
+
+    P_fit[slice_frac], residual, threshold_lower, threshold_upper, \
+    master_mask[slice_frac] = GaussianSmoothing2D(
+        X, Y, P_obs[slice_frac], sigma=(0, sigma), m=mask_arr[slice_frac], 
+        maxiters=maxiters, sigma_lower=sigma_lower, sigma_upper=sigma_upper, axis=1, 
+        grow=grow, use_relative=False)
+
+    # Non-negative
+    P_fit = np.max(np.stack([P_fit, np.zeros_like(P_fit)]), axis=0)
+    # Normalization
+    P_fit /= P_fit.sum(axis=0)
+
+    # Plot
+    _validateBool(show, 'show')
+    _validateBool(save, 'save')
+
+    if show | save:
+
+        _validateString(title, 'title')
+        if title != 'profile':
+            title = f'{title} profile'
+
+        fig, ax = plt.subplots(1, 1, dpi=100)
+
+        _plot2d(ax=ax, ccd=P_fit, cmap='Greys_r', contrast=0.25, aspect='auto')
+        (xmin, xmax), (ymin, ymax) = ax.get_xlim(), ax.get_ylim()
+        if slit_along == 'col':
+            for profile_edge in profile_edges:
+                ax.axhline(y=profile_edge, ls='--', color='r', lw=1.5)
+        else:
+            for profile_edge in profile_edges:
+                ax.axvline(x=profile_edge, ls='--', color='r', lw=1.5)
+
+        # Settings
+        ax.set_xlim(xmin, xmax)
+        ax.set_ylim(ymin, ymax)
+        ax.set_title(title, fontsize=16)
+        fig.set_figheight(n_row / n_col * fig.get_figwidth())
+        fig.tight_layout()
+
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
+
+        if show:
+            plt.show()
+
+        plt.close()
+
+    if save:
+
+        fig_path = _validatePath(path, f'{title} fitting', '.pdf')
+        with PdfPages(fig_path, keep_empty=False) as pdf:
+
+            for i in idx_frac:
+
+                fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
+                fig.subplots_adjust(hspace=0)
+
+                _plotFitting(
+                    ax=ax, x=idx_col, y=P_obs[slice_frac][i], 
+                    m=master_mask[slice_frac][i], x_fit=idx_col, 
+                    y_fit=P_fit[slice_frac][i], r=residual[i], 
+                    threshold_lower=threshold_lower[i], 
+                    threshold_upper=threshold_upper[i], xlabel='dispersion axis [px]', 
+                    ylabel='fraction', use_relative=False)
+
+                # Settings
+                ax[0].set_title(f'profile at row {idx_row[slice_frac][i]}', fontsize=16)
+
+                fig.align_ylabels()
+                fig.tight_layout()
+
+                pdf.savefig(fig, dpi=100)
+
+                plt.close()
+
+    nccd.mask = master_mask.copy()
+
+    # Output
+    if isinstance(ccd, CCDData):
+        nccd.header['PROFILE'] = '{} Uncertainty and mask refined.'.format(
+            Time.now().to_value('iso', subfmt='date_hm'))
+
+    elif np.ma.isMaskedArray(ccd):
+        nccd = np.ma.array(nccd.data, mask=nccd.mask)
+
+    else:
+        nccd = nccd.data.copy()
+
+    return P_fit, nccd
+
+
+def extract(ccd, slit_along, method, trace1d=None, aper_width=None, n_aper=None, 
+            profile2d=None, background2d=None, rdnoise=None, maxiters=None, 
+            sigma_lower=None, sigma_upper=None, grow=None, spectral_axis=None, 
+            use_uncertainty=True, use_mask=True, title='aperture', show=conf.fig_show, 
             save=conf.fig_save, path=conf.fig_path):
     """Extract 1-dimensional spectra.
     
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
     
     slit_along : str
         `col` or `row`. If `row`, the data array of ``ccd`` will be transposed during 
         calculations. Note that this will NOT affect the returned trace.
     
-    trace1d : `~specutils.Spectrum1D` or scalar or `~numpy.ndarray`
-        Input trace.
-    
-    aper_width : scalar or 2-tuple
-        Aperture width.
-    
     method : str
-        Extraction method. `optimal` or `sum`, and
-        - if `optimal`, the optimal extraction algorithm will be used. The spatial 
-        profile will be normalized to unity within ``psf_width``, and then pixels 
-        within ``aper_width`` will be used to compute the source flux. Only one 
-        spectrum will be extracted regardless of ``n_aper``.
-        - if `sum`, the source flux from the pixels within ``aper_width`` will be 
-        summed.
-    
-    psf_width : scalar or 2-tuple or `None`, optional
-        Width of the point spread function (used by the optimal extraction algorithm). 
-        If `None`, it will be set equal to ``aper_width``.
+        Extraction method. `sum` or `optimal`, and
+        - if `sum`, the source flux from the pixels within an aperture defined by 
+        ``trace1d`` and ``aper_width`` are summed. The ``n_aper`` argument allows the 
+        users to divide the whole aperture into several sub-apertures.
+        - if `optimal`, the optimal extraction algorithm will be used. The normalized 
+        spatial profile is used to compute the source flux. The sky background and 
+        readout noise are used to estimate variance iteratively. ``n_aper`` is ignored.
+
+    trace1d : `~specutils.Spectrum1D` or scalar or `~numpy.ndarray` or `None`, optional
+        Input trace (used by summation extraction algorithm).
     
-    n_aper : int, optional
+    aper_width : scalar or 2-tuple or `None`, optional
+        Aperture width (used by summation extraction algorithm).
+
+    n_aper : int or `None`, optional
         Number of sub-apertures (used by the summation extraction algorithm).
         Default is `1`.
 
+    profile2d : `~numpy.ndarray` or `None`, optional
+        Spatial profile (used by the optimal extraction algorithm).
+
+    background2d : `~numpy.ndarray`
+        Pre-modeled sky background of ``ccd``. Used to estimate variance iteratively. 
+        Note that this sky background should have already been subtraced from ``ccd``.
+
+    rdnoise : scalar
+        Readout noise of ``ccd``. Used to estimate variance iteratively.
+
+    maxiters : int, optional
+        Maximum number of sigma-clipping iterations to perform. If convergence is 
+        achieved prior to ``maxiters`` iterations, the clipping iterations will stop. 
+        Must be >= `0`. 
+        Default is `5`.
+
+    sigma_lower : scalar or `None`, optional
+        Number of standard deviations to use as the lower bound for the clipping limit. 
+        If `None` (default), `3` is used.
+
+    sigma_upper : scalar or `None`, optional
+        Number of standard deviations to use as the upper bound for the clipping limit. 
+        If `None` (default), `3` is used.
+    
+    grow : scalar or `False`, optional
+        Radius within which to mask the neighbouring pixels of those that fall outwith 
+        the clipping limits.
+
     spectral_axis : `~astropy.units.Quantity` or `None`
         Spectral axis of the extracted 1-dimensional spectra.
 
+    use_uncertainty : bool, optional
+        If `True` and an uncertainty array is attributed to ``ccd``, the uncertainties 
+        are used as weights in the fitting. 
+        Default is `False`.
+
+    use_mask : bool, optional
+        If `True` and a mask array is attributed to ``ccd``, the masked pixels are 
+        ignored in the fitting. 
+        Default is `False`.
+
     Returns
     -------
     spectrum1d : `~specutils.Spectrum1D`
         Extracted 1-dimensional spectra.
     """
 
     _validateString(slit_along, 'slit_along', ['col', 'row'])
     
     if slit_along == 'col':
         nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
-            ccd, 'ccd', True, True, False)
+            ccd, 'ccd', use_uncertainty, use_mask, False)
     else:
         nccd, data_arr, uncertainty_arr, mask_arr = _validateCCD(
-            ccd, 'ccd', True, True, True)
+            ccd, 'ccd', use_uncertainty, use_mask, True)
 
     n_row, n_col = data_arr.shape
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
-    # Assume that unit of the trace is [pixel]
-    if isinstance(trace1d, Spectrum1D):
-        trace1d = trace1d.flux.value
-    trace1d = _validate1DArray(trace1d, 'trace1d', n_col, True)
-    
-    # The total aperture width is the sum of ``aper_width[0]`` and ``aper_width[1]``. 
-    # If they have opposite signs, the whole aperture will be on one side of the trace.
-    aper_width = _validateAperture(aper_width, 'aper_width')
-    aper_width[0] *= -1; aper_width.sort()
-    
-    _validateString(method, 'method', ['optimal', 'sum'])
-    
-    if method == 'optimal':
-        
-        if psf_width is None:
-            psf_width = aper_width
-        else:
-            psf_width = _validateAperture(psf_width, 'psf_width')
-            psf_width[0] *= -1; psf_width.sort()
-            if (psf_width[0] > aper_width[0]) | (psf_width[1] < aper_width[1]):
-                raise ValueError('``aper_width`` should be <= ``psf_width.')
-        
-        psf_edges = np.vstack([np.round(trace1d).astype(int) + round(psf_width[0]), 
-                               np.round(trace1d).astype(int) + round(psf_width[1])]).T
-        
-        psf_arr = np.zeros(((psf_edges[0][1] - psf_edges[0][0] + 1), n_col))
-        for i, psf_edge in enumerate(psf_edges):
-            psf_arr[:, i] = data_arr[psf_edge[0]:(psf_edge[1] + 1), i]
-        
-        # aper_edges = trace1d + np.array([aper_width[0], aper_width[1]])[:, np.newaxis]
-        print(psf_arr)
-        
-    else:
+    _validateString(method, 'method', ['sum', 'optimal'])
+
+    variance_arr = uncertainty_arr**2
+
+    if method == 'sum':
+
+        # Assume that unit of the trace is [pixel]
+        if isinstance(trace1d, Spectrum1D):
+            trace1d = trace1d.flux.value
+        trace1d = _validate1DArray(trace1d, 'trace1d', n_col, True)
+
+        # The total aperture width is the sum of the two elements of ``aper_width``. If 
+        # they have opposite signs, the whole aperture will be on the same side of the 
+        # trace.
+        aper_width = _validateAperture(aper_width, 'aper_width')
+        aper_width[0] *= -1; aper_width.sort()
         
         _validateInteger(n_aper, 'n_aper', (1, None), (True, None))
         
         aper_edges = trace1d + np.linspace(
             aper_width[0], aper_width[1], n_aper + 1)[:, np.newaxis]
 
         # Out-of-range problem can be ignored in background modeling while cannot here.
         if (aper_edges.min() < -0.5) | (aper_edges.max() > n_row - 0.5):
             raise ValueError('Aperture edge is out of range.')
 
         data_aper = np.zeros((n_aper, n_col))
-
-        uncertainty_aper = np.zeros((n_aper, n_col)) # !!! Variance !!!
-
+        variance_aper = np.zeros((n_aper, n_col))
         mask_aper = np.zeros((n_aper, n_col), dtype=bool)
 
         for i in idx_col:
 
             aper_start, aper_end = aper_edges[:-1, i], aper_edges[1:, i]
 
             for j in range(n_aper):
 
                 # Internal pixels
                 mask = (aper_start[j] < idx_row - 0.5) & (idx_row + 0.5 < aper_end[j])
                 data_aper[j, i] = data_arr[mask, i].sum()
-                uncertainty_aper[j, i] = np.sum(uncertainty_arr[mask, i]**2)
+                variance_aper[j, i] = np.sum(variance_arr[mask, i])
                 mask_aper[j, i] = np.any(mask_arr[mask, i])
 
                 # Edge pixels
 
                 # ``idx_start`` labels the pixel where ``aper_start`` is in
                 idx_start = idx_row[idx_row - 0.5 <= aper_start[j]][-1]
 
                 # ``idx_end`` labels the pixel where ``aper_end`` is in
                 idx_end = idx_row[idx_row + 0.5 >= aper_end[j]][0]
 
                 # ``aper_start`` and ``aper_end`` are in the same pixel
                 if idx_start == idx_end:
                     data_aper[j, i] += (
                         data_arr[idx_end, i] * (aper_end[j] - aper_start[j]))
-                    uncertainty_aper[j, i] += (
-                        uncertainty_arr[idx_end, i] * (aper_end[j] - aper_start[j]))**2
+                    variance_aper[j, i] += (
+                        variance_arr[idx_end, i] * (aper_end[j] - aper_start[j])**2)
                     mask_aper[j, i] |= mask_arr[idx_end, i]
 
                 # in different pixels
                 else:
                     data_aper[j, i] += (
                         data_arr[idx_start, i] * (idx_start + 0.5 - aper_start[j])
                         + data_arr[idx_end, i] * (aper_end[j] - (idx_end - 0.5))
                     )
-                    uncertainty_aper[j, i] += (
-                        (uncertainty_arr[idx_start, i]
-                         * (idx_start + 0.5 - aper_start[j]))**2 
-                        + (uncertainty_arr[idx_end, i] 
-                           * (aper_end[j] - (idx_end - 0.5)))**2
+                    variance_aper[j, i] += (
+                        (variance_arr[idx_start, i]
+                         * (idx_start + 0.5 - aper_start[j])**2)
+                        + (variance_arr[idx_end, i] 
+                           * (aper_end[j] - (idx_end - 0.5))**2)
                     )
                     mask_aper[j, i] |= mask_arr[idx_start, i] | mask_arr[idx_end, i]
 
-        uncertainty_aper = np.sqrt(uncertainty_aper) # Standard deviation
+        uncertainty_aper = np.sqrt(variance_aper)
+    
+    else:
 
-    _validateBool(show, 'show')
+        # P -- spatial profile (Horne 1986)
+        P = _validateNDArray(profile2d, 'profile2d', data_arr.ndim)
+        # S -- sky background (Horne 1986)
+        S = _validateNDArray(background2d, 'background2d', data_arr.ndim)
+        if not (data_arr.shape == P.shape == S.shape):
+            raise ValueError(
+                'The input frame, the spatial profile, and the sky background should '
+                'have the same shape.'
+            )
+
+        _validateRange(rdnoise, 'rdnoise', (0, None), (True, None))
+
+        _validateInteger(maxiters, 'maxiters', (0, None), (True, None))
+
+        # V -- variance (Horne 1986)
+        V_inverse = (1 / variance_arr) if use_uncertainty else (1 + variance_arr)
+        # In case of zero variance
+        V_inverse[~np.isfinite(V_inverse)] = 0
+
+        # M -- cosmic ray mask (Horne 1986)
+        M_new = (~mask_arr) & (P > 0)
+        M_old = np.zeros_like(M_new, dtype=bool)
 
-    _validateString(title, 'title')
-    if title != 'aperture':
-        title = f'{title} aperture'
+        k = 0
+        while np.any(M_new != M_old) & (k <= maxiters):
+
+            M_old = M_new.copy()
+
+            # f = (Σ M x (D-S)/P x P^2/V) / (Σ M x P^2/V) --- optimal object flux 
+            # (Horne 1986)
+            f = np.sum(M_old * data_arr * P * V_inverse, axis=0) / \
+                np.sum(M_old * P**2 * V_inverse, axis=0)
+
+            # var[f] = (Σ M x P) / (Σ M x P^2/V) --- variance of optimal 
+            # object flux (Horne 1986)
+            var_f = np.sum(M_old * P, axis=0) / np.sum(M_old * P**2 * V_inverse, axis=0)
+            
+            # Update
+            V_inverse = 1 / (rdnoise**2 + np.abs(f * P + S))
 
-    fig_path = _validatePath(save, path, title)
+            # Standardized residual
+            residual = (data_arr - f * P) * np.sqrt(V_inverse)
+
+            if maxiters == 0:
+                threshold_lower, threshold_upper = None, None
+
+            elif k < maxiters:
+                residual[(mask_arr | (P == 0))] = np.nan
+                residual_masked, threshold_lower, threshold_upper = sigma_clip(
+                    data=residual, sigma_lower=sigma_lower, sigma_upper=sigma_upper, 
+                    maxiters=1, stdfunc='mad_std', axis=None, masked=True, 
+                    return_bounds=True, grow=grow)
+                M_new = ~residual_masked.mask
+
+            k += 1
+
+        data_aper = f[np.newaxis, :]
+        uncertainty_aper = np.sqrt(var_f)[np.newaxis, :]
+        mask_aper = np.zeros_like(data_aper, dtype=bool)
+        
+        aper_edges = np.zeros((2, n_col))
+        for i in idx_col:
+            aper_edges[:, i] = np.where(P[:, i] > 0)[0][[0, -1]]
+
+    # Plot
+    _validateBool(show, 'show')
+    _validateBool(save, 'save')
 
     if show | save:
 
-        extent = (-0.5, nccd.shape[1] - 0.5, -0.5, nccd.shape[0] - 0.5)
+        _validateString(title, 'title')
+        if title != 'aperture':
+            title = f'{title} aperture'
 
-        fig = plt.figure(dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
-        _plot2d(ax=ax, ccd=nccd.data, cmap='Greys_r', contrast=0.25, extent=extent)
+        fig, ax = plt.subplots(1, 1, dpi=100)
+
+        _plot2d(ax=ax, ccd=data_arr, cmap='Greys_r', contrast=0.25, aspect='auto')
         (xmin, xmax), (ymin, ymax) = ax.get_xlim(), ax.get_ylim()
         if slit_along == 'col':
             for aper_edge in aper_edges:
                 ax.plot(idx_col, aper_edge, 'r--', lw=1.5)
         else:
             for aper_edge in aper_edges:
-                ax.plot(aper_edge, idx_row, 'r--', lw=1.5)
+                ax.plot(aper_edge, idx_col, 'r--', lw=1.5)
+
         # Settings
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
         ax.set_title(title, fontsize=16)
+        fig.set_figheight(n_row / n_col * fig.get_figwidth())
         fig.tight_layout()
 
-        if save: plt.savefig(fig_path, dpi=100)
+        if save:
+            fig_path = _validatePath(path, title)
+            plt.savefig(fig_path, dpi=100)
 
-        if show: plt.show()
+        if show:
+            plt.show()
 
         plt.close()
 
     # Output
     spectrum1d = Spectrum1D(
         spectral_axis=spectral_axis, flux=(data_aper * nccd.unit), 
         uncertainty=StdDevUncertainty(uncertainty_aper), mask=mask_aper, 
@@ -1797,15 +2102,15 @@
 
     wavelength_sens = new_sens1d.wavelength.value
 
     # Extinction curve
     if extinct is not None:
 
         if isinstance(airmass, str):
-            airmass = spectrum1d.meta['header'][airmass]
+            airmass = ccd.meta[airmass]
 
         if isinstance(extinct, str):
             spectrum_ext = loadExtinctionCurve(extinct)
 
         elif isinstance(extinct, Spectrum1D):
             spectrum_ext = deepcopy(extinct)
 
@@ -1893,10 +2198,10 @@
         calibrated_ccd.header['CALIBRAT'] = '{} Calibrated'.format(
             Time.now().to_value('iso', subfmt='date_hm'))
 
     elif np.ma.isMaskedArray(ccd):
         calibrated_ccd = np.ma.array(calibrated_ccd.data, mask=calibrated_ccd.mask)
 
     else:
-        calibrated_ccd = deepcopy(calibrated_ccd.data)
+        calibrated_ccd = calibrated_ccd.data.copy()
 
     return calibrated_ccd
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/twodspec/utils.py` & `astro-drpy-0.0.1.7/src/drpy/twodspec/utils.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.6/src/drpy/utils.py` & `astro-drpy-0.0.1.7/src/drpy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,14 @@
             [file_name, ccd.shape, np.mean(ccd.data), np.std(ccd.data, ddof=1), 
              np.min(ccd.data), np.max(ccd.data)])
 
     stats = Table(rows=rows, names=['IMAGE', 'SHAPE', 'MEAN', 'STDDEV', 'MIN', 'MAX'])
     
     # Format
     for colname in ['MEAN', 'STDDEV', 'MIN', 'MAX']:
-        stats[colname].format = "g"
+        stats[colname].format = 'g'
 
     _validateBool(verbose, 'verbose')
 
     if verbose: stats.pprint_all()
 
     return stats
```

### Comparing `astro-drpy-0.0.1.6/src/drpy/validate.py` & `astro-drpy-0.0.1.7/src/drpy/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     if not isinstance(ccd, (np.ndarray, CCDData)):
         raise TypeError('Invalid type `{}` for ``{}``.'.format(type(ccd), name))
     # May have (or not have) uncertainty frame or mask frame.
     elif isinstance(ccd, CCDData):
         nccd = ccd.copy()
     # Do not have uncertainty frame. May have (or not have) mask frame.
     else:
-        nccd = CCDData(deepcopy(ccd), unit=unit_ccddata)
+        nccd = CCDData(ccd.copy(), unit=unit_ccddata)
 
     return nccd
 
 
 def _validateSpectrum1D(spectrum, name):
     """Validate a spectrum."""
 
@@ -294,42 +294,44 @@
 
     else:
         raise TypeError(f'Invalid type `{type(ccdlist)}` for ``ccdlist``.')
     
     return nccdlist
 
 
-def _validateCCD(ccd, name, use_uncertainty, use_mask, transpose):
+def _validateCCD(ccd, name, use_uncertainty, use_mask, transpose, asWeight=False):
     """Validate a CCD image."""
     
     nccd = _validateCCDData(ccd, name)
 
     # Data
-    data_arr = deepcopy(nccd.data)
+    data_arr = nccd.data.copy()
     
     # Uncertainty
     if use_uncertainty:
         if nccd.uncertainty is None:
             warnings.warn(
                 'The input uncertainty is unavailable. All set to zero.', 
                 RuntimeWarning)
-            uncertainty_arr = np.zeros_like(data_arr)
+            uncertainty_arr = (
+                np.zeros_like(data_arr) if not asWeight else np.ones_like(data_arr))
         else:
-            uncertainty_arr = deepcopy(nccd.uncertainty.array)
+            uncertainty_arr = nccd.uncertainty.array.copy()
     else:
-        uncertainty_arr = np.zeros_like(data_arr)
+        uncertainty_arr = (
+            np.zeros_like(data_arr) if not asWeight else np.ones_like(data_arr))
     
     # Mask
     if use_mask:
         if nccd.mask is None:
             warnings.warn(
                 'The input mask is unavailable. All set unmasked.', RuntimeWarning)
             mask_arr = np.zeros_like(data_arr, dtype=bool)
         else:
-            mask_arr = deepcopy(nccd.mask)
+            mask_arr = nccd.mask.copy()
     else:
         mask_arr = np.zeros_like(data_arr, dtype=bool)
 
     if transpose:
         data_arr = data_arr.T
         uncertainty_arr = uncertainty_arr.T
         mask_arr = mask_arr.T
@@ -339,67 +341,72 @@
 
 def _validateSpectrum(spectrum, name, use_uncertainty, use_mask):
     """Validate a spectrum."""
 
     new_spectrum = _validateSpectrum1D(spectrum, name)
     
     # Data
-    spectral_axis = deepcopy(new_spectrum.spectral_axis.value)
-    flux = deepcopy(new_spectrum.flux.value)
+    spectral_axis = new_spectrum.spectral_axis.value.copy()
+    flux = new_spectrum.flux.value.copy()
     
     # Uncertainty
     if use_uncertainty:
         if new_spectrum.uncertainty is None:
             warnings.warn(
                 'The input uncertainty is unavailable. All set to zero.', 
                 RuntimeWarning)
             uncertainty = np.zeros_like(flux)
         else:
-            uncertainty = deepcopy(new_spectrum.uncertainty.array)
+            uncertainty = new_spectrum.uncertainty.array.copy()
     else:
         uncertainty = np.zeros_like(flux)
     
     # Mask
     if use_mask:
         if new_spectrum.mask is None:
             warnings.warn(
                 'The input mask is unavailable. All set unmasked.', RuntimeWarning)
             mask = np.zeros_like(flux, dtype=bool)
         else:
-            mask = deepcopy(new_spectrum.mask)
+            mask = new_spectrum.mask.copy()
     else:
         mask = np.zeros_like(flux, dtype=bool)
     
     return new_spectrum, spectral_axis, flux, uncertainty, mask
 
 
-def _validateBins(bins, length):
+def _validateBins(bins, length, isWidth=False):
     """Validate bins and derive bin edges."""
 
     if np.ndim(bins) == 0:
         # Validate
         _validateInteger(bins, 'bins', (1, length), (True, True))
         # Generate bin edges
-        bin_edges = np.linspace(0, length, bins + 1).astype(int)
+        if isWidth:
+            bin_edges = np.hstack([np.arange(0, length, bins), length])
+        else:
+            bin_edges = np.linspace(0, length, bins + 1).astype(int)
 
     elif np.ndim(bins) == 1:
         # Generate bin edges
         bin_edges = np.array(bins).astype(int)
         # Validate
         _validateInteger(bin_edges.min(), 'bin_edges', (0, length), (True, True))
         _validateInteger(bin_edges.max(), 'bin_edges', (0, length), (True, True))
         if np.any(bin_edges[:-1] > bin_edges[1:]):
             raise ValueError('``bins`` must increase monotonically, when an array')
 
     else:
         raise ValueError('``bins`` must be 1-dimensional, when an array')
 
     bin_edges = np.vstack([bin_edges[:-1], bin_edges[1:]]).T
+    n_bin = bin_edges.shape[0]
+    loc_bin = (bin_edges.sum(axis=1) - 1) / 2
 
-    return bin_edges
+    return bin_edges, loc_bin, n_bin
 
 
 def _validateAperture(aperture, name):
     """Validate aperture width."""
 
     if np.ndim(aperture) == 0:
 
@@ -415,25 +422,23 @@
             aperture.sum(), f'{name}.sum()', (0, None), (False, None))
 
     else:
         raise ValueError(f'``{name}`` must be 1-dimensional, when an array')
 
     return aperture
 
-
-def _validatePath(save, path, title, extension='.png'):
+# todo: slugify
+def _validatePath(path, title, extension='.png'):
     """Validate path arguments."""
 
-    _validateBool(save, 'save')
-
     if path is None:
         path = os.getcwd()
 
-    else:
-        _validateString(path, 'path')
+    elif not os.path.exists(path):
+        raise OSError(f'Path {path} does not exist.')
 
     if isinstance(title, str):
         fig_name = f'{title}{extension}'.replace(' ', '_')
         fig_path = os.path.join(path, fig_name)
 
     else:
         fig_path = list()
```

