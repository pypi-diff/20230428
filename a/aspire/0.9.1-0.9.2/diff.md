# Comparing `tmp/aspire-0.9.1.tar.gz` & `tmp/aspire-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspire-0.9.1.tar", last modified: Fri Apr 15 18:04:22 2022, max compression
+gzip compressed data, was "dist/aspire-0.9.2.tar", last modified: Thu Jun  2 16:06:38 2022, max compression
```

## Comparing `aspire-0.9.1.tar` & `aspire-0.9.2.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/
--rw-r--r--   0 carmichael   (502) staff       (20)      602 2022-04-15 17:53:36.000000 aspire-0.9.1/.bumpversion.cfg
--rw-r--r--   0 carmichael   (502) staff       (20)      287 2022-04-15 17:53:36.000000 aspire-0.9.1/.codecov.yml
--rw-r--r--   0 carmichael   (502) staff       (20)       72 2022-04-15 17:53:36.000000 aspire-0.9.1/.git-blame-ignore-revs
--rw-r--r--   0 carmichael   (502) staff       (20)     1319 2022-04-15 17:53:36.000000 aspire-0.9.1/CODEOWNERS
--rw-r--r--   0 carmichael   (502) staff       (20)     3354 2022-04-15 17:53:36.000000 aspire-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 carmichael   (502) staff       (20)     5750 2022-04-15 17:53:36.000000 aspire-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 carmichael   (502) staff       (20)     4095 2022-04-15 17:53:36.000000 aspire-0.9.1/CONTRIBUTORS.rst
--rw-r--r--   0 carmichael   (502) staff       (20)    32473 2022-04-15 17:53:36.000000 aspire-0.9.1/LICENSE
--rw-r--r--   0 carmichael   (502) staff       (20)      494 2022-04-15 17:53:36.000000 aspire-0.9.1/MANIFEST.in
--rw-r--r--   0 carmichael   (502) staff       (20)     4679 2022-04-15 18:04:22.000000 aspire-0.9.1/PKG-INFO
--rw-r--r--   0 carmichael   (502) staff       (20)     4046 2022-04-15 17:53:36.000000 aspire-0.9.1/README.md
--rw-r--r--   0 carmichael   (502) staff       (20)     3169 2022-04-15 17:53:36.000000 aspire-0.9.1/azure-pipelines.yml
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/docs/
--rw-r--r--   0 carmichael   (502) staff       (20)      841 2022-04-15 17:53:36.000000 aspire-0.9.1/docs/Makefile
--rwxr-xr-x   0 carmichael   (502) staff       (20)     1386 2022-04-15 17:53:36.000000 aspire-0.9.1/docs/buildsite.sh
--rw-r--r--   0 carmichael   (502) staff       (20)      769 2022-04-15 17:53:36.000000 aspire-0.9.1/docs/make.bat
--rw-r--r--   0 carmichael   (502) staff       (20)      120 2022-04-15 17:53:36.000000 aspire-0.9.1/environment.yml
--rw-r--r--   0 carmichael   (502) staff       (20)       38 2022-04-15 18:04:22.000000 aspire-0.9.1/setup.cfg
--rw-r--r--   0 carmichael   (502) staff       (20)     2365 2022-04-15 17:53:36.000000 aspire-0.9.1/setup.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/
--rw-r--r--   0 carmichael   (502) staff       (20)     1029 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)      708 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/__main__.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/abinitio/
--rw-r--r--   0 carmichael   (502) staff       (20)      127 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    22818 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_base.py
--rw-r--r--   0 carmichael   (502) staff       (20)      578 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_ev.py
--rw-r--r--   0 carmichael   (502) staff       (20)      823 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_gcar.py
--rw-r--r--   0 carmichael   (502) staff       (20)      748 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_lud.py
--rw-r--r--   0 carmichael   (502) staff       (20)      586 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_sdp.py
--rw-r--r--   0 carmichael   (502) staff       (20)    18684 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/commonline_sync.py
--rw-r--r--   0 carmichael   (502) staff       (20)      714 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/abinitio/orientation_src.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/apple/
--rw-r--r--   0 carmichael   (502) staff       (20)       25 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/apple/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    12123 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/apple/apple.py
--rw-r--r--   0 carmichael   (502) staff       (20)    10352 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/apple/helper.py
--rw-r--r--   0 carmichael   (502) staff       (20)    18249 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/apple/picking.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/basis/
--rw-r--r--   0 carmichael   (502) staff       (20)      494 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     8022 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/basis.py
--rw-r--r--   0 carmichael   (502) staff       (20)    13445 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/basis_utils.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2820 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/dirac.py
--rw-r--r--   0 carmichael   (502) staff       (20)    15335 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/fb_2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     8054 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/fb_3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     9989 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/ffb_2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)    14730 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/ffb_3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)    13369 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/fpswf_2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)       89 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/fpswf_3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)    21530 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/fspca.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4619 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/polar_2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)    13950 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/pswf_2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)       68 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/pswf_3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     5118 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/pswf_utils.py
--rw-r--r--   0 carmichael   (502) staff       (20)     7504 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/basis/steerable.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/classification/
--rw-r--r--   0 carmichael   (502) staff       (20)      272 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/classification/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    37648 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/classification/averager2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1555 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/classification/class2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4711 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/classification/legacy_implementations.py
--rw-r--r--   0 carmichael   (502) staff       (20)    20889 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/classification/rir_class2d.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/commands/
--rw-r--r--   0 carmichael   (502) staff       (20)        0 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)      321 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/_config.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3763 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/apple.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1979 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/cov3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3163 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/denoise.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2053 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/estimate_ctf.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4491 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/extract_particles.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2211 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/orient3d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3049 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/commands/preprocess.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/config/
--rw-r--r--   0 carmichael   (502) staff       (20)     2654 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/config/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)      562 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/config.ini
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/covariance/
--rw-r--r--   0 carmichael   (502) staff       (20)      100 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/covariance/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     8063 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/covariance/covar.py
--rw-r--r--   0 carmichael   (502) staff       (20)    30725 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/covariance/covar2d.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/ctf/
--rwxr-xr-x   0 carmichael   (502) staff       (20)       54 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/ctf/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    28567 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/ctf/ctf_estimator.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/denoising/
--rw-r--r--   0 carmichael   (502) staff       (20)      185 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3726 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/adaptive_support.py
--rw-r--r--   0 carmichael   (502) staff       (20)      531 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/class_avg.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2101 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/denoised_src.py
--rw-r--r--   0 carmichael   (502) staff       (20)      814 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/denoiser.py
--rw-r--r--   0 carmichael   (502) staff       (20)     7322 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/denoising/denoiser_cov2d.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3259 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/exceptions.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/image/
--rw-r--r--   0 carmichael   (502) staff       (20)      216 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/image/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    12604 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/image/image.py
--rw-r--r--   0 carmichael   (502) staff       (20)     7434 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/image/preprocess.py
--rw-r--r--   0 carmichael   (502) staff       (20)    17055 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/image/xform.py
--rw-r--r--   0 carmichael   (502) staff       (20)      547 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/logging.conf
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/noise/
--rw-r--r--   0 carmichael   (502) staff       (20)       82 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/noise/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4841 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/noise/noise.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/nufft/
--rw-r--r--   0 carmichael   (502) staff       (20)     8636 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/nufft/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     6533 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/nufft/cufinufft.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4817 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/nufft/finufft.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2230 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/nufft/pynfft.py
--rw-r--r--   0 carmichael   (502) staff       (20)       93 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/nufft/utils.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/numeric/
--rw-r--r--   0 carmichael   (502) staff       (20)      865 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2334 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/base_fft.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/numeric/complex_pca/
--rw-r--r--   0 carmichael   (502) staff       (20)        0 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/complex_pca/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2775 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/complex_pca/complex_pca.py
--rw-r--r--   0 carmichael   (502) staff       (20)    18242 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/complex_pca/validation.py
--rw-r--r--   0 carmichael   (502) staff       (20)      229 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/cupy.py
--rw-r--r--   0 carmichael   (502) staff       (20)      936 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/cupy_fft.py
--rw-r--r--   0 carmichael   (502) staff       (20)      284 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/numpy.py
--rw-r--r--   0 carmichael   (502) staff       (20)     4419 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/pyfftw_fft.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1031 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/numeric/scipy_fft.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/operators/
--rw-r--r--   0 carmichael   (502) staff       (20)      403 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/operators/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    27704 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/operators/blk_diag_matrix.py
--rw-r--r--   0 carmichael   (502) staff       (20)    15351 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/operators/filters.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3325 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/operators/wemd.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/optimization/
--rw-r--r--   0 carmichael   (502) staff       (20)       46 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/optimization/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     6925 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/optimization/conj_grad.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/reconstruction/
--rw-r--r--   0 carmichael   (502) staff       (20)      107 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/reconstruction/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     5235 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/reconstruction/estimator.py
--rw-r--r--   0 carmichael   (502) staff       (20)     5302 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/reconstruction/kernel.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1670 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/reconstruction/mean.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/source/
--rw-r--r--   0 carmichael   (502) staff       (20)      295 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)    23386 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/coordinates.py
--rw-r--r--   0 carmichael   (502) staff       (20)    31420 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/image.py
--rw-r--r--   0 carmichael   (502) staff       (20)      583 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/mrcstack.py
--rw-r--r--   0 carmichael   (502) staff       (20)    10778 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/relion.py
--rw-r--r--   0 carmichael   (502) staff       (20)    13212 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/source/simulation.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/storage/
--rw-r--r--   0 carmichael   (502) staff       (20)      107 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/storage/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     3709 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/storage/micrograph.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1597 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/storage/mrc.py
--rw-r--r--   0 carmichael   (502) staff       (20)     8892 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/storage/starfile.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/utils/
--rw-r--r--   0 carmichael   (502) staff       (20)      840 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/__init__.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1458 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/cell.py
--rw-r--r--   0 carmichael   (502) staff       (20)    10528 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/coor_trans.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2883 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/fft.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2111 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/filter_to_fb_mat.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1879 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/matlab_compat.py
--rw-r--r--   0 carmichael   (502) staff       (20)    13786 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/matrix.py
--rw-r--r--   0 carmichael   (502) staff       (20)     6695 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/misc.py
--rw-r--r--   0 carmichael   (502) staff       (20)     2722 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/random.py
--rw-r--r--   0 carmichael   (502) staff       (20)    10150 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/rotation.py
--rw-r--r--   0 carmichael   (502) staff       (20)     1926 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/utils/types.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire/volume/
--rw-r--r--   0 carmichael   (502) staff       (20)    18297 2022-04-15 17:53:36.000000 aspire-0.9.1/src/aspire/volume/__init__.py
-drwxr-xr-x   0 carmichael   (502) staff       (20)        0 2022-04-15 18:04:22.000000 aspire-0.9.1/src/aspire.egg-info/
--rw-r--r--   0 carmichael   (502) staff       (20)     4679 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/PKG-INFO
--rw-r--r--   0 carmichael   (502) staff       (20)     4016 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/SOURCES.txt
--rw-r--r--   0 carmichael   (502) staff       (20)        1 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/dependency_links.txt
--rw-r--r--   0 carmichael   (502) staff       (20)       54 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/entry_points.txt
--rw-r--r--   0 carmichael   (502) staff       (20)      427 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/requires.txt
--rw-r--r--   0 carmichael   (502) staff       (20)        7 2022-04-15 18:04:21.000000 aspire-0.9.1/src/aspire.egg-info/top_level.txt
--rw-r--r--   0 carmichael   (502) staff       (20)        1 2022-04-15 18:01:14.000000 aspire-0.9.1/src/aspire.egg-info/zip-safe
--rw-r--r--   0 carmichael   (502) staff       (20)     2133 2022-04-15 17:53:36.000000 aspire-0.9.1/tox.ini
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/
+-rw-r--r--   0 gbwright   (502) staff       (20)      602 2022-06-02 11:01:12.000000 aspire-0.9.2/.bumpversion.cfg
+-rw-r--r--   0 gbwright   (502) staff       (20)      287 2021-09-07 13:14:30.000000 aspire-0.9.2/.codecov.yml
+-rw-r--r--   0 gbwright   (502) staff       (20)       72 2021-09-07 13:14:30.000000 aspire-0.9.2/.git-blame-ignore-revs
+-rw-r--r--   0 gbwright   (502) staff       (20)     1255 2022-05-13 19:36:25.000000 aspire-0.9.2/.zenodo.json
+-rw-r--r--   0 gbwright   (502) staff       (20)     1319 2021-09-07 13:14:30.000000 aspire-0.9.2/CODEOWNERS
+-rw-r--r--   0 gbwright   (502) staff       (20)     3354 2021-09-07 13:14:30.000000 aspire-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 gbwright   (502) staff       (20)     5750 2021-11-12 13:01:11.000000 aspire-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 gbwright   (502) staff       (20)     4095 2022-05-13 19:36:25.000000 aspire-0.9.2/CONTRIBUTORS.rst
+-rw-r--r--   0 gbwright   (502) staff       (20)    32473 2021-09-07 13:14:30.000000 aspire-0.9.2/LICENSE
+-rw-r--r--   0 gbwright   (502) staff       (20)      515 2022-05-13 19:36:25.000000 aspire-0.9.2/MANIFEST.in
+-rw-r--r--   0 gbwright   (502) staff       (20)     4679 2022-06-02 16:06:38.000000 aspire-0.9.2/PKG-INFO
+-rw-r--r--   0 gbwright   (502) staff       (20)     4046 2022-06-02 11:01:12.000000 aspire-0.9.2/README.md
+-rw-r--r--   0 gbwright   (502) staff       (20)     3169 2022-02-22 14:24:41.000000 aspire-0.9.2/azure-pipelines.yml
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/docs/
+-rw-r--r--   0 gbwright   (502) staff       (20)      841 2021-11-12 13:01:11.000000 aspire-0.9.2/docs/Makefile
+-rwxr-xr-x   0 gbwright   (502) staff       (20)     1386 2021-09-07 13:14:30.000000 aspire-0.9.2/docs/buildsite.sh
+-rw-r--r--   0 gbwright   (502) staff       (20)      769 2021-09-07 13:14:30.000000 aspire-0.9.2/docs/make.bat
+-rw-r--r--   0 gbwright   (502) staff       (20)      120 2022-02-22 14:24:41.000000 aspire-0.9.2/environment.yml
+-rw-r--r--   0 gbwright   (502) staff       (20)       38 2022-06-02 16:06:38.000000 aspire-0.9.2/setup.cfg
+-rw-r--r--   0 gbwright   (502) staff       (20)     2365 2022-06-02 11:01:12.000000 aspire-0.9.2/setup.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/
+-rw-r--r--   0 gbwright   (502) staff       (20)     1029 2022-06-02 11:01:12.000000 aspire-0.9.2/src/aspire/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      708 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/__main__.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/abinitio/
+-rw-r--r--   0 gbwright   (502) staff       (20)      127 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    22818 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/abinitio/commonline_base.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      578 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/commonline_ev.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      823 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/commonline_gcar.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      748 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/commonline_lud.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      586 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/commonline_sdp.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    18684 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/abinitio/commonline_sync.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      714 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/abinitio/orientation_src.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/apple/
+-rw-r--r--   0 gbwright   (502) staff       (20)       25 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/apple/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    12123 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/apple/apple.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    10352 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/apple/helper.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    18260 2022-06-02 11:01:07.000000 aspire-0.9.2/src/aspire/apple/picking.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/basis/
+-rw-r--r--   0 gbwright   (502) staff       (20)      523 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     6511 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/basis/basis.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    13445 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/basis/basis_utils.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2820 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/dirac.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1819 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/fb.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    15363 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/fb_2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     8082 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/fb_3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     9989 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/ffb_2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    14730 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/ffb_3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    13369 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/fpswf_2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)       89 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/basis/fpswf_3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    21530 2021-11-12 13:01:11.000000 aspire-0.9.2/src/aspire/basis/fspca.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4619 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/basis/polar_2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    13950 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/basis/pswf_2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)       68 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/basis/pswf_3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     5118 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/basis/pswf_utils.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     7504 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/basis/steerable.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/classification/
+-rw-r--r--   0 gbwright   (502) staff       (20)      272 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/classification/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    37648 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/classification/averager2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1555 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/classification/class2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4711 2021-11-12 13:01:11.000000 aspire-0.9.2/src/aspire/classification/legacy_implementations.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    20889 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/classification/rir_class2d.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/commands/
+-rw-r--r--   0 gbwright   (502) staff       (20)        0 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/commands/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      321 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/commands/_config.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3763 2022-02-22 14:24:41.000000 aspire-0.9.2/src/aspire/commands/apple.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1979 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/commands/cov3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3163 2021-11-12 13:01:11.000000 aspire-0.9.2/src/aspire/commands/denoise.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2053 2021-10-05 18:04:43.000000 aspire-0.9.2/src/aspire/commands/estimate_ctf.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4491 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/commands/extract_particles.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2211 2022-02-22 14:24:41.000000 aspire-0.9.2/src/aspire/commands/orient3d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3049 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/commands/preprocess.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/config/
+-rw-r--r--   0 gbwright   (502) staff       (20)     2654 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/config/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      562 2022-02-22 14:24:41.000000 aspire-0.9.2/src/aspire/config.ini
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/covariance/
+-rw-r--r--   0 gbwright   (502) staff       (20)      100 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/covariance/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     8063 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/covariance/covar.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    30725 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/covariance/covar2d.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/ctf/
+-rwxr-xr-x   0 gbwright   (502) staff       (20)       54 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/ctf/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    28567 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/ctf/ctf_estimator.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/denoising/
+-rw-r--r--   0 gbwright   (502) staff       (20)      185 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/denoising/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3726 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/denoising/adaptive_support.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      531 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/denoising/class_avg.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2101 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/denoising/denoised_src.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      814 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/denoising/denoiser.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     7322 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/denoising/denoiser_cov2d.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3259 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/exceptions.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/image/
+-rw-r--r--   0 gbwright   (502) staff       (20)      216 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/image/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    12026 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/image/image.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     7434 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/image/preprocess.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    17055 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/image/xform.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      547 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/logging.conf
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/noise/
+-rw-r--r--   0 gbwright   (502) staff       (20)       82 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/noise/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4841 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/noise/noise.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/nufft/
+-rw-r--r--   0 gbwright   (502) staff       (20)     8636 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/nufft/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     6533 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/nufft/cufinufft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4817 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/nufft/finufft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2230 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/nufft/pynfft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)       93 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/nufft/utils.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/numeric/
+-rw-r--r--   0 gbwright   (502) staff       (20)      865 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2334 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/base_fft.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/numeric/complex_pca/
+-rw-r--r--   0 gbwright   (502) staff       (20)        0 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/complex_pca/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2775 2022-05-23 15:38:51.000000 aspire-0.9.2/src/aspire/numeric/complex_pca/complex_pca.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    18080 2022-06-02 11:01:07.000000 aspire-0.9.2/src/aspire/numeric/complex_pca/validation.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      229 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/cupy.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      936 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/cupy_fft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      284 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/numpy.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     4419 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/pyfftw_fft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1031 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/numeric/scipy_fft.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/operators/
+-rw-r--r--   0 gbwright   (502) staff       (20)      403 2022-02-22 14:24:40.000000 aspire-0.9.2/src/aspire/operators/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    27704 2021-09-20 19:16:34.000000 aspire-0.9.2/src/aspire/operators/blk_diag_matrix.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    15351 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/operators/filters.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3325 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/operators/wemd.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/optimization/
+-rw-r--r--   0 gbwright   (502) staff       (20)       46 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/optimization/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     6925 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/optimization/conj_grad.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/reconstruction/
+-rw-r--r--   0 gbwright   (502) staff       (20)      107 2021-11-12 13:39:00.000000 aspire-0.9.2/src/aspire/reconstruction/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     5235 2022-05-13 19:36:25.000000 aspire-0.9.2/src/aspire/reconstruction/estimator.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     5302 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/reconstruction/kernel.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1670 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/reconstruction/mean.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/source/
+-rw-r--r--   0 gbwright   (502) staff       (20)      295 2022-02-22 14:25:49.000000 aspire-0.9.2/src/aspire/source/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    23386 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/source/coordinates.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    31420 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/source/image.py
+-rw-r--r--   0 gbwright   (502) staff       (20)      583 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/source/mrcstack.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    10778 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/source/relion.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    13212 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/source/simulation.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/storage/
+-rw-r--r--   0 gbwright   (502) staff       (20)      107 2021-10-05 18:04:43.000000 aspire-0.9.2/src/aspire/storage/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     3750 2022-06-02 11:01:07.000000 aspire-0.9.2/src/aspire/storage/micrograph.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1597 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/storage/mrc.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     8892 2021-11-12 13:01:11.000000 aspire-0.9.2/src/aspire/storage/starfile.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/utils/
+-rw-r--r--   0 gbwright   (502) staff       (20)      840 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/utils/__init__.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1458 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/utils/cell.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    10528 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/utils/coor_trans.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2883 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/utils/fft.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2111 2021-12-09 17:27:42.000000 aspire-0.9.2/src/aspire/utils/filter_to_fb_mat.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1879 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/utils/matlab_compat.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    13786 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/utils/matrix.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     6695 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/utils/misc.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     2722 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/utils/random.py
+-rw-r--r--   0 gbwright   (502) staff       (20)    10150 2022-02-22 14:25:50.000000 aspire-0.9.2/src/aspire/utils/rotation.py
+-rw-r--r--   0 gbwright   (502) staff       (20)     1926 2021-09-07 13:14:30.000000 aspire-0.9.2/src/aspire/utils/types.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire/volume/
+-rw-r--r--   0 gbwright   (502) staff       (20)    18297 2022-05-13 19:37:19.000000 aspire-0.9.2/src/aspire/volume/__init__.py
+drwxr-xr-x   0 gbwright   (502) staff       (20)        0 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/
+-rw-r--r--   0 gbwright   (502) staff       (20)     4679 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/PKG-INFO
+-rw-r--r--   0 gbwright   (502) staff       (20)     4052 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/SOURCES.txt
+-rw-r--r--   0 gbwright   (502) staff       (20)        1 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/dependency_links.txt
+-rw-r--r--   0 gbwright   (502) staff       (20)       55 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/entry_points.txt
+-rw-r--r--   0 gbwright   (502) staff       (20)      427 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/requires.txt
+-rw-r--r--   0 gbwright   (502) staff       (20)        7 2022-06-02 16:06:38.000000 aspire-0.9.2/src/aspire.egg-info/top_level.txt
+-rw-r--r--   0 gbwright   (502) staff       (20)        1 2021-10-12 17:56:37.000000 aspire-0.9.2/src/aspire.egg-info/zip-safe
+-rw-r--r--   0 gbwright   (502) staff       (20)     2180 2022-05-13 19:36:25.000000 aspire-0.9.2/tox.ini
```

### Comparing `aspire-0.9.1/.bumpversion.cfg` & `aspire-0.9.2/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.1
+current_version = 0.9.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `aspire-0.9.1/CODEOWNERS` & `aspire-0.9.2/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/CODE_OF_CONDUCT.md` & `aspire-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/CONTRIBUTING.md` & `aspire-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/CONTRIBUTORS.rst` & `aspire-0.9.2/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/LICENSE` & `aspire-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/PKG-INFO` & `aspire-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspire
-Version: 0.9.1
+Version: 0.9.2
 Summary: Algorithms for Single Particle Reconstruction
 Home-page: https://github.com/ComputationalCryoEM/ASPIRE-Python
 Author: Joakim Anden, Ayelet Heimowitz, Vineet Bansal, Robbie Brook, Itay Sason, Yoel Shkolnisky, Garrett Wright, Junchao Xia
 Author-email: devs.aspire@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -18,30 +18,30 @@
 ![Logo](http://spr.math.princeton.edu/sites/spr.math.princeton.edu/files/ASPIRE_1.jpg)
 
 [![Azure Build Status](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_apis/build/status/ComputationalCryoEM.ASPIRE-Python?branchName=master)](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_build/latest?definitionId=3&branchName=master)
 [![Github Actions Status](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml/badge.svg)](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python/branch/master/graph/badge.svg?token=3XFC4VONX0)](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5657281.svg)](https://doi.org/10.5281/zenodo.5657281)
 
-# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.1
+# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.2
 
 This is the Python version to supersede the [Matlab ASPIRE](https://github.com/PrincetonUniversity/aspire).
 
 ASPIRE is an open-source software package for processing single-particle cryo-EM data to determine three-dimensional structures of biological macromolecules. The package includes advanced algorithms based on rigorous mathematics and recent developments in
 statistics and machine learning. It provides unique and improved solutions to important computational challenges of the cryo-EM
 processing pipeline, including 3-D *ab-initio* modeling, 2-D class averaging, automatic particle picking, and 3-D heterogeneity analysis.
 
 For more information about the project, algorithms, and related publications please refer to the [ASPIRE Project website](http://spr.math.princeton.edu/).
 
 **For full documentation and tutorials see [the docs](https://computationalcryoem.github.io/ASPIRE-Python).**
 
 Please cite using the following DOI. This DOI represents all versions, and will always resolve to the latest one.
 
 ```
-ComputationalCryoEM/ASPIRE-Python: v0.9.1 https://doi.org/10.5281/zenodo.5657281
+ComputationalCryoEM/ASPIRE-Python: v0.9.2 https://doi.org/10.5281/zenodo.5657281
 
 ```
 
 ## Installation Instructions
 
 For end-users
 -------------
```

### Comparing `aspire-0.9.1/README.md` & `aspire-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ![Logo](http://spr.math.princeton.edu/sites/spr.math.princeton.edu/files/ASPIRE_1.jpg)
 
 [![Azure Build Status](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_apis/build/status/ComputationalCryoEM.ASPIRE-Python?branchName=master)](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_build/latest?definitionId=3&branchName=master)
 [![Github Actions Status](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml/badge.svg)](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python/branch/master/graph/badge.svg?token=3XFC4VONX0)](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5657281.svg)](https://doi.org/10.5281/zenodo.5657281)
 
-# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.1
+# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.2
 
 This is the Python version to supersede the [Matlab ASPIRE](https://github.com/PrincetonUniversity/aspire).
 
 ASPIRE is an open-source software package for processing single-particle cryo-EM data to determine three-dimensional structures of biological macromolecules. The package includes advanced algorithms based on rigorous mathematics and recent developments in
 statistics and machine learning. It provides unique and improved solutions to important computational challenges of the cryo-EM
 processing pipeline, including 3-D *ab-initio* modeling, 2-D class averaging, automatic particle picking, and 3-D heterogeneity analysis.
 
 For more information about the project, algorithms, and related publications please refer to the [ASPIRE Project website](http://spr.math.princeton.edu/).
 
 **For full documentation and tutorials see [the docs](https://computationalcryoem.github.io/ASPIRE-Python).**
 
 Please cite using the following DOI. This DOI represents all versions, and will always resolve to the latest one.
 
 ```
-ComputationalCryoEM/ASPIRE-Python: v0.9.1 https://doi.org/10.5281/zenodo.5657281
+ComputationalCryoEM/ASPIRE-Python: v0.9.2 https://doi.org/10.5281/zenodo.5657281
 
 ```
 
 ## Installation Instructions
 
 For end-users
 -------------
```

### Comparing `aspire-0.9.1/azure-pipelines.yml` & `aspire-0.9.2/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/docs/Makefile` & `aspire-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/docs/buildsite.sh` & `aspire-0.9.2/docs/buildsite.sh`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/docs/make.bat` & `aspire-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/setup.py` & `aspire-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="aspire",
-    version="0.9.1",
+    version="0.9.2",
     data_files=[
         ("", ["src/aspire/config.ini"]),
         ("", ["src/aspire/logging.conf"]),
     ],
     include_package_data=True,
     description="Algorithms for Single Particle Reconstruction",
     long_description=read("README.md"),
```

### Comparing `aspire-0.9.1/src/aspire/__init__.py` & `aspire-0.9.2/src/aspire/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 import aspire
 from aspire.config import Config
 from aspire.exceptions import handle_exception
 
 # version in maj.min.bld format
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # Implements some code that writes out exceptions to 'aspire.err.log'.
 config = Config(read_text(aspire, "config.ini"))
 if config.logging.log_exceptions:
     import sys
 
     sys.excepthook = handle_exception
```

### Comparing `aspire-0.9.1/src/aspire/__main__.py` & `aspire-0.9.2/src/aspire/__main__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_base.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_base.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_ev.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_ev.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_gcar.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_gcar.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_lud.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_lud.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_sdp.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_sdp.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/commonline_sync.py` & `aspire-0.9.2/src/aspire/abinitio/commonline_sync.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/abinitio/orientation_src.py` & `aspire-0.9.2/src/aspire/abinitio/orientation_src.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/apple/apple.py` & `aspire-0.9.2/src/aspire/apple/apple.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/apple/helper.py` & `aspire-0.9.2/src/aspire/apple/helper.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/apple/picking.py` & `aspire-0.9.2/src/aspire/apple/picking.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,17 +187,17 @@
         # Make square
         side_length = min(im.shape)
         im = im[:side_length, :side_length]
 
         size = tuple((np.array(im.shape) / self.mrc_shrink_factor).astype(int))
 
         # Note, float64 required for signal.correlate call accuracy.
-        im = np.asarray(Image.fromarray(im).resize(size, Image.BICUBIC)).astype(
-            np.float64, copy=False
-        )
+        im = np.asarray(
+            Image.fromarray(im).resize(size, Image.Resampling.BICUBIC)
+        ).astype(np.float64, copy=False)
 
         im = signal.correlate(
             im,
             PickerHelper.gaussian_filter(
                 self.mrc_gauss_filter_size, self.mrc_gauss_filter_sigma
             ),
             "same",
```

### Comparing `aspire-0.9.1/src/aspire/basis/basis.py` & `aspire-0.9.2/src/aspire/basis/basis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 
 import numpy as np
 from scipy.sparse.linalg import LinearOperator, cg
 
-from aspire.basis.basis_utils import num_besselj_zeros
 from aspire.image import Image
 from aspire.utils import mdim_mat_fun_conj
-from aspire.utils.matlab_compat import m_reshape
 from aspire.volume import Volume
 
 logger = logging.getLogger(__name__)
 
 
 class Basis:
     """
@@ -43,54 +41,14 @@
         if self.dtype not in (np.float32, np.float64):
             raise NotImplementedError(
                 "Currently only implemented for float32 and float64 types"
             )
 
         self._build()
 
-    def _getfbzeros(self):
-        """
-        Generate zeros of Bessel functions
-        """
-        # get upper_bound of zeros of Bessel functions
-        upper_bound = min(self.ell_max + 1, 2 * self.nres + 1)
-
-        # List of number of zeros
-        n = []
-        # List of zero values (each entry is an ndarray; all of possibly different lengths)
-        zeros = []
-
-        # generate zeros of Bessel functions for each ell
-        for ell in range(upper_bound):
-            # for each ell, num_besselj_zeros returns the zeros of the
-            # order ell Bessel function which are less than 2*pi*c*R = nres*pi/2,
-            # the truncation rule for the Fourier-Bessel expansion
-            _n, _zeros = num_besselj_zeros(
-                ell + (self.ndim - 2) / 2, self.nres * np.pi / 2
-            )
-            if _n == 0:
-                break
-            else:
-                n.append(_n)
-                zeros.append(_zeros)
-
-        #  get maximum number of ell
-        self.ell_max = len(n) - 1
-
-        #  set the maximum of k for each ell
-        self.k_max = np.array(n, dtype=int)
-
-        max_num_zeros = max(len(z) for z in zeros)
-        for i, z in enumerate(zeros):
-            zeros[i] = np.hstack(
-                (z, np.zeros(max_num_zeros - len(z), dtype=self.dtype))
-            )
-
-        self.r0 = m_reshape(np.hstack(zeros), (-1, self.ell_max + 1)).astype(self.dtype)
-
     def _build(self):
         """
         Build the internal data structure to represent basis
         """
         raise NotImplementedError("subclasses must implement this")
 
     def indices(self):
```

### Comparing `aspire-0.9.1/src/aspire/basis/basis_utils.py` & `aspire-0.9.2/src/aspire/basis/basis_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         else:
             # Some predictions were off, set to double the number of good predictions
             j = 2 * (np.where(abs(err) >= err_tol)[0][0] + 1)
 
     return z
 
 
-def num_besselj_zeros(ell, r):
+def all_besselj_zeros(ell, r):
     """
     Compute the zeros of the order `ell` Bessel function which are less than `r`.
 
     :param ell: The real number order of the Bessel function.
     :param r: The upper bound for zeros returned.
     :return n, r0: The number of zeros and the zeros themselves
     as a NumPy array.
```

### Comparing `aspire-0.9.1/src/aspire/basis/dirac.py` & `aspire-0.9.2/src/aspire/basis/dirac.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/fb_2d.py` & `aspire-0.9.2/src/aspire/basis/fb_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 
 import numpy as np
 from scipy.special import jv
 
-from aspire.basis import SteerableBasis2D
+from aspire.basis import FBBasisMixin, SteerableBasis2D
 from aspire.basis.basis_utils import unique_coords_nd
 from aspire.image import Image
 from aspire.utils import complex_type, real_type, roll_dim, unroll_dim
 from aspire.utils.matlab_compat import m_flatten, m_reshape
 
 logger = logging.getLogger(__name__)
 
 
-class FBBasis2D(SteerableBasis2D):
+class FBBasis2D(SteerableBasis2D, FBBasisMixin):
     """
     Define a derived class using the Fourier-Bessel basis for mapping 2D images
 
     The expansion coefficients of 2D images on this basis are obtained by
     the least squares method. The algorithm is described in the publication:
     Z. Zhao, A. Singer, Fourier-Bessel Rotational Invariant Eigenimages,
     The Journal of the Optical Society of America A, 30 (5), pp. 871-877 (2013).
@@ -50,15 +50,15 @@
         """
         logger.info(
             "Expanding 2D images in a spatial-domain Fourier–Bessel"
             " basis using the direct method."
         )
 
         # get upper bound of zeros, ells, and ks  of Bessel functions
-        self._getfbzeros()
+        self._calc_k_max()
 
         # calculate total number of basis functions
         self.count = self.k_max[0] + sum(2 * self.k_max[1:])
 
         # obtain a 2D grid to represent basis functions
         self.basis_coords = unique_coords_nd(self.nres, self.ndim, dtype=self.dtype)
```

### Comparing `aspire-0.9.1/src/aspire/basis/fb_3d.py` & `aspire-0.9.2/src/aspire/basis/fb_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 
 import numpy as np
 
-from aspire.basis import Basis
+from aspire.basis import Basis, FBBasisMixin
 from aspire.basis.basis_utils import real_sph_harmonic, sph_bessel, unique_coords_nd
 from aspire.utils import roll_dim, unroll_dim
 from aspire.utils.matlab_compat import m_flatten, m_reshape
 
 logger = logging.getLogger(__name__)
 
 
-class FBBasis3D(Basis):
+class FBBasis3D(Basis, FBBasisMixin):
     """
     Define a derived class for direct spherical Harmonics Bessel basis expanding 3D volumes
 
     # TODO: Methods that return dictionaries should return useful objects instead
 
     """
 
@@ -45,15 +45,15 @@
 
         logger.info(
             "Expanding 3D map in a spatial-domain Fourier–Bessel"
             " basis using the direct method."
         )
 
         # get upper bound of zeros, ells, and ks  of Bessel functions
-        self._getfbzeros()
+        self._calc_k_max()
 
         # calculate total number of basis functions
         self.count = sum(self.k_max * (2 * np.arange(0, self.ell_max + 1) + 1))
 
         # obtain a 3D grid to represent basis functions
         self.basis_coords = unique_coords_nd(self.nres, self.ndim, dtype=self.dtype)
```

### Comparing `aspire-0.9.1/src/aspire/basis/ffb_2d.py` & `aspire-0.9.2/src/aspire/basis/ffb_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.rcut = self.nres / 2
         self.kcut = 0.5
         self.n_r = int(np.ceil(4 * self.rcut * self.kcut))
         n_theta = np.ceil(16 * self.kcut * self.rcut)
         self.n_theta = int((n_theta + np.mod(n_theta, 2)) / 2)
 
         # get upper bound of zeros, ells, and ks  of Bessel functions
-        self._getfbzeros()
+        self._calc_k_max()
 
         # calculate total number of basis functions
         self.count = self.k_max[0] + sum(2 * self.k_max[1:])
 
         # generate 1D indices for basis functions
         self._compute_indices()
         self._indices = self.indices()
```

### Comparing `aspire-0.9.1/src/aspire/basis/ffb_3d.py` & `aspire-0.9.2/src/aspire/basis/ffb_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         )
 
         # set cutoff values
         self.rcut = self.nres / 2
         self.kcut = 0.5
 
         # get upper bound of zeros, ells, and ks  of Bessel functions
-        self._getfbzeros()
+        self._calc_k_max()
 
         # calculate total number of basis functions
         self.count = sum(self.k_max * (2 * np.arange(0, self.ell_max + 1) + 1))
 
         # generate 1D indices for basis functions
         self._indices = self.indices()
```

### Comparing `aspire-0.9.1/src/aspire/basis/fpswf_2d.py` & `aspire-0.9.2/src/aspire/basis/fpswf_2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/fspca.py` & `aspire-0.9.2/src/aspire/basis/fspca.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/polar_2d.py` & `aspire-0.9.2/src/aspire/basis/polar_2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/pswf_2d.py` & `aspire-0.9.2/src/aspire/basis/pswf_2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/pswf_utils.py` & `aspire-0.9.2/src/aspire/basis/pswf_utils.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/basis/steerable.py` & `aspire-0.9.2/src/aspire/basis/steerable.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/classification/averager2d.py` & `aspire-0.9.2/src/aspire/classification/averager2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/classification/class2d.py` & `aspire-0.9.2/src/aspire/classification/class2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/classification/legacy_implementations.py` & `aspire-0.9.2/src/aspire/classification/legacy_implementations.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/classification/rir_class2d.py` & `aspire-0.9.2/src/aspire/classification/rir_class2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/apple.py` & `aspire-0.9.2/src/aspire/commands/apple.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/cov3d.py` & `aspire-0.9.2/src/aspire/commands/cov3d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/denoise.py` & `aspire-0.9.2/src/aspire/commands/denoise.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/estimate_ctf.py` & `aspire-0.9.2/src/aspire/commands/estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/extract_particles.py` & `aspire-0.9.2/src/aspire/commands/extract_particles.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/orient3d.py` & `aspire-0.9.2/src/aspire/commands/orient3d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/commands/preprocess.py` & `aspire-0.9.2/src/aspire/commands/preprocess.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/config/__init__.py` & `aspire-0.9.2/src/aspire/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/config.ini` & `aspire-0.9.2/src/aspire/config.ini`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/covariance/covar.py` & `aspire-0.9.2/src/aspire/covariance/covar.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/covariance/covar2d.py` & `aspire-0.9.2/src/aspire/covariance/covar2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/ctf/ctf_estimator.py` & `aspire-0.9.2/src/aspire/ctf/ctf_estimator.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/denoising/adaptive_support.py` & `aspire-0.9.2/src/aspire/denoising/adaptive_support.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/denoising/class_avg.py` & `aspire-0.9.2/src/aspire/denoising/class_avg.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/denoising/denoised_src.py` & `aspire-0.9.2/src/aspire/denoising/denoised_src.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/denoising/denoiser.py` & `aspire-0.9.2/src/aspire/denoising/denoiser.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/denoising/denoiser_cov2d.py` & `aspire-0.9.2/src/aspire/denoising/denoiser_cov2d.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/exceptions.py` & `aspire-0.9.2/src/aspire/exceptions.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/image/image.py` & `aspire-0.9.2/src/aspire/image/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 
 import matplotlib.pyplot as plt
 import mrcfile
 import numpy as np
-from scipy.interpolate import RegularGridInterpolator
 from scipy.linalg import lstsq
 
 import aspire.volume
 from aspire.nufft import anufft
 from aspire.numeric import fft, xp
-from aspire.utils import grid_2d
+from aspire.utils import crop_pad_2d, grid_2d
 from aspire.utils.matrix import anorm
 
 logger = logging.getLogger(__name__)
 
 
 def _im_translate2(im, shifts):
     """
@@ -205,38 +204,22 @@
         """
         Downsample Image to a specific resolution. This method returns a new Image.
 
         :param ds_res: int - new resolution, should be <= the current resolution
             of this Image
         :return: The downsampled Image object.
         """
-        grid = grid_2d(self.res, indexing="yx")
-        grid_ds = grid_2d(ds_res, indexing="yx")
+        # compute FT with centered 0-frequency
+        fx = fft.centered_fft2(self.data)
+        # crop 2D Fourier transform for each image
+        crop_fx = np.array([crop_pad_2d(fx[i], ds_res) for i in range(self.n_images)])
+        # take back to real space, discard complex part, and scale
+        out = np.real(fft.centered_ifft2(crop_fx)) * (ds_res**2 / self.res**2)
 
-        im_ds = np.zeros((self.n_images, ds_res, ds_res), dtype=self.dtype)
-
-        # x, y values corresponding to 'grid'. This is what scipy interpolator needs to function.
-        res_by_2 = self.res / 2
-        x = y = np.ceil(np.arange(-res_by_2, res_by_2)) / res_by_2
-
-        mask = (np.abs(grid["x"]) < ds_res / self.res) & (
-            np.abs(grid["y"]) < ds_res / self.res
-        )
-        im_shifted = fft.centered_ifft2(
-            fft.centered_fft2(xp.asarray(self.data)) * xp.asarray(mask)
-        )
-        im = np.real(xp.asnumpy(im_shifted))
-
-        for s in range(im_ds.shape[0]):
-            interpolator = RegularGridInterpolator(
-                (x, y), im[s], bounds_error=False, fill_value=0
-            )
-            im_ds[s] = interpolator(np.dstack([grid_ds["y"], grid_ds["x"]]))
-
-        return Image(im_ds)
+        return Image(out)
 
     def filter(self, filter):
         """
         Apply a `Filter` object to the Image and returns a new Image.
 
         :param filter: An object of type `Filter`.
         :return: A new filtered `Image` object.
```

### Comparing `aspire-0.9.1/src/aspire/image/preprocess.py` & `aspire-0.9.2/src/aspire/image/preprocess.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/image/xform.py` & `aspire-0.9.2/src/aspire/image/xform.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/logging.conf` & `aspire-0.9.2/src/aspire/logging.conf`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/noise/noise.py` & `aspire-0.9.2/src/aspire/noise/noise.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/nufft/__init__.py` & `aspire-0.9.2/src/aspire/nufft/__init__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/nufft/cufinufft.py` & `aspire-0.9.2/src/aspire/nufft/cufinufft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/nufft/finufft.py` & `aspire-0.9.2/src/aspire/nufft/finufft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/nufft/pynfft.py` & `aspire-0.9.2/src/aspire/nufft/pynfft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/__init__.py` & `aspire-0.9.2/src/aspire/numeric/__init__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/base_fft.py` & `aspire-0.9.2/src/aspire/numeric/base_fft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/complex_pca/complex_pca.py` & `aspire-0.9.2/src/aspire/numeric/complex_pca/complex_pca.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/complex_pca/validation.py` & `aspire-0.9.2/src/aspire/numeric/complex_pca/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,19 @@
 
 import numbers
 import warnings
 
 import numpy as np
 import scipy.sparse as sp
 from numpy.core.numeric import ComplexWarning
-from sklearn.exceptions import DataConversionWarning, NonBLASDotWarning
+from sklearn.exceptions import DataConversionWarning
 from sklearn.utils.validation import _assert_all_finite
 
 FLOAT_DTYPES = (np.float64, np.float32, np.float16)
 
-# Silenced by default to reduce verbosity. Turn on at runtime for
-# performance profiling.
-warnings.simplefilter("ignore", NonBLASDotWarning)
-
 
 def _num_samples(x):
     """Return number of samples in array-like x."""
     message = "Expected sequence or array-like, got %s" % type(x)
     if hasattr(x, "fit") and callable(x.fit):
         # Don't get num_samples from an ensembles length!
         raise TypeError(message)
```

### Comparing `aspire-0.9.1/src/aspire/numeric/cupy_fft.py` & `aspire-0.9.2/src/aspire/numeric/cupy_fft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/pyfftw_fft.py` & `aspire-0.9.2/src/aspire/numeric/pyfftw_fft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/numeric/scipy_fft.py` & `aspire-0.9.2/src/aspire/numeric/scipy_fft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/operators/blk_diag_matrix.py` & `aspire-0.9.2/src/aspire/operators/blk_diag_matrix.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/operators/filters.py` & `aspire-0.9.2/src/aspire/operators/filters.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/operators/wemd.py` & `aspire-0.9.2/src/aspire/operators/wemd.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/optimization/conj_grad.py` & `aspire-0.9.2/src/aspire/optimization/conj_grad.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/reconstruction/estimator.py` & `aspire-0.9.2/src/aspire/reconstruction/estimator.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/reconstruction/kernel.py` & `aspire-0.9.2/src/aspire/reconstruction/kernel.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/reconstruction/mean.py` & `aspire-0.9.2/src/aspire/reconstruction/mean.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/source/coordinates.py` & `aspire-0.9.2/src/aspire/source/coordinates.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/source/image.py` & `aspire-0.9.2/src/aspire/source/image.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/source/mrcstack.py` & `aspire-0.9.2/src/aspire/source/mrcstack.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/source/relion.py` & `aspire-0.9.2/src/aspire/source/relion.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/source/simulation.py` & `aspire-0.9.2/src/aspire/source/simulation.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/storage/micrograph.py` & `aspire-0.9.2/src/aspire/storage/micrograph.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,17 @@
 
         if self.square:
             side_length = min(im.shape[-2], im.shape[-1])
             im = im[..., :side_length, :side_length]
 
         if self.shrink_factor is not None:
             size = tuple((np.array(im.shape) / self.shrink_factor).astype(int))
-            im = np.array(PILImage.fromarray(im).resize(size, PILImage.BICUBIC))
+            im = np.array(
+                PILImage.fromarray(im).resize(size, PILImage.Resampling.BICUBIC)
+            )
 
         if self.gauss_filter_size is not None:
             im = signal.correlate(
                 im,
                 Micrograph.gaussian_filter(
                     self.gauss_filter_size, self.gauss_filter_sigma
                 ),
```

### Comparing `aspire-0.9.1/src/aspire/storage/mrc.py` & `aspire-0.9.2/src/aspire/storage/mrc.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/storage/starfile.py` & `aspire-0.9.2/src/aspire/storage/starfile.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/__init__.py` & `aspire-0.9.2/src/aspire/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/cell.py` & `aspire-0.9.2/src/aspire/utils/cell.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/coor_trans.py` & `aspire-0.9.2/src/aspire/utils/coor_trans.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/fft.py` & `aspire-0.9.2/src/aspire/utils/fft.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/filter_to_fb_mat.py` & `aspire-0.9.2/src/aspire/utils/filter_to_fb_mat.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/matlab_compat.py` & `aspire-0.9.2/src/aspire/utils/matlab_compat.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/matrix.py` & `aspire-0.9.2/src/aspire/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/misc.py` & `aspire-0.9.2/src/aspire/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/random.py` & `aspire-0.9.2/src/aspire/utils/random.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/rotation.py` & `aspire-0.9.2/src/aspire/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/utils/types.py` & `aspire-0.9.2/src/aspire/utils/types.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire/volume/__init__.py` & `aspire-0.9.2/src/aspire/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aspire-0.9.1/src/aspire.egg-info/PKG-INFO` & `aspire-0.9.2/src/aspire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspire
-Version: 0.9.1
+Version: 0.9.2
 Summary: Algorithms for Single Particle Reconstruction
 Home-page: https://github.com/ComputationalCryoEM/ASPIRE-Python
 Author: Joakim Anden, Ayelet Heimowitz, Vineet Bansal, Robbie Brook, Itay Sason, Yoel Shkolnisky, Garrett Wright, Junchao Xia
 Author-email: devs.aspire@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -18,30 +18,30 @@
 ![Logo](http://spr.math.princeton.edu/sites/spr.math.princeton.edu/files/ASPIRE_1.jpg)
 
 [![Azure Build Status](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_apis/build/status/ComputationalCryoEM.ASPIRE-Python?branchName=master)](https://dev.azure.com/ComputationalCryoEM/Aspire-Python/_build/latest?definitionId=3&branchName=master)
 [![Github Actions Status](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml/badge.svg)](https://github.com/ComputationalCryoEM/ASPIRE-Python/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python/branch/master/graph/badge.svg?token=3XFC4VONX0)](https://codecov.io/gh/ComputationalCryoEM/ASPIRE-Python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5657281.svg)](https://doi.org/10.5281/zenodo.5657281)
 
-# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.1
+# ASPIRE - Algorithms for Single Particle Reconstruction - v0.9.2
 
 This is the Python version to supersede the [Matlab ASPIRE](https://github.com/PrincetonUniversity/aspire).
 
 ASPIRE is an open-source software package for processing single-particle cryo-EM data to determine three-dimensional structures of biological macromolecules. The package includes advanced algorithms based on rigorous mathematics and recent developments in
 statistics and machine learning. It provides unique and improved solutions to important computational challenges of the cryo-EM
 processing pipeline, including 3-D *ab-initio* modeling, 2-D class averaging, automatic particle picking, and 3-D heterogeneity analysis.
 
 For more information about the project, algorithms, and related publications please refer to the [ASPIRE Project website](http://spr.math.princeton.edu/).
 
 **For full documentation and tutorials see [the docs](https://computationalcryoem.github.io/ASPIRE-Python).**
 
 Please cite using the following DOI. This DOI represents all versions, and will always resolve to the latest one.
 
 ```
-ComputationalCryoEM/ASPIRE-Python: v0.9.1 https://doi.org/10.5281/zenodo.5657281
+ComputationalCryoEM/ASPIRE-Python: v0.9.2 https://doi.org/10.5281/zenodo.5657281
 
 ```
 
 ## Installation Instructions
 
 For end-users
 -------------
```

### Comparing `aspire-0.9.1/src/aspire.egg-info/SOURCES.txt` & `aspire-0.9.2/src/aspire.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .bumpversion.cfg
 .codecov.yml
 .git-blame-ignore-revs
+.zenodo.json
 CODEOWNERS
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 CONTRIBUTORS.rst
 LICENSE
 MANIFEST.in
 README.md
@@ -39,14 +40,15 @@
 src/aspire/apple/apple.py
 src/aspire/apple/helper.py
 src/aspire/apple/picking.py
 src/aspire/basis/__init__.py
 src/aspire/basis/basis.py
 src/aspire/basis/basis_utils.py
 src/aspire/basis/dirac.py
+src/aspire/basis/fb.py
 src/aspire/basis/fb_2d.py
 src/aspire/basis/fb_3d.py
 src/aspire/basis/ffb_2d.py
 src/aspire/basis/ffb_3d.py
 src/aspire/basis/fpswf_2d.py
 src/aspire/basis/fpswf_3d.py
 src/aspire/basis/fspca.py
```

### Comparing `aspire-0.9.1/tox.ini` & `aspire-0.9.2/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     isort
     twine
 skip_install = true
 commands =
     flake8 .
     isort --check-only --diff .
     black --check --diff .
+    python -m json.tool .zenodo.json /dev/null
     check-manifest .
     python setup.py sdist
     twine check dist/*.*
 
 [flake8]
 # The following for recomended for use with Black
 max-line-length = 88
```

