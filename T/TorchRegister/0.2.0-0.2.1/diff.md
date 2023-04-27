# Comparing `tmp/TorchRegister-0.2.0.tar.gz` & `tmp/TorchRegister-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchRegister-0.2.0.tar", last modified: Thu Apr 27 22:32:41 2023, max compression
+gzip compressed data, was "TorchRegister-0.2.1.tar", last modified: Thu Apr 27 23:14:19 2023, max compression
```

## Comparing `TorchRegister-0.2.0.tar` & `TorchRegister-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.714936 TorchRegister-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.714936 TorchRegister-0.2.0/src/TorchRegister/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/torchregister.py
--rw-r--r--   0 runner    (1001) docker     (123)    15689 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/warpings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/src/TorchRegister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.148772 TorchRegister-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/src/TorchRegister/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/torchregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-27 23:14:08.000000 TorchRegister-0.2.1/src/TorchRegister/warpings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:14:19.152772 TorchRegister-0.2.1/src/TorchRegister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 23:14:19.000000 TorchRegister-0.2.1/src/TorchRegister.egg-info/top_level.txt
```

### Comparing `TorchRegister-0.2.0/LICENSE.md` & `TorchRegister-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.2.0/README.md` & `TorchRegister-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.2.0/setup.py` & `TorchRegister-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TorchRegister',
-    version='0.2.0',
+    version='0.2.1',
     url='https://github.com/AgamChopra/TorchRegister',
     author='Agam Chopra',
     author_email='achopra4@uw.edu',
     description='3D image registration methods for PyTorch.',
     long_description='Common medical 3D image registration methods such as rigid, affine, and flow field for PyTorch.',
     install_requires=['torch >= 2.0.0', 'numpy >= 1.24.1',
                       'tqdm >= 4.65.0', 'matplotlib  >= 3.7.1'],
```

### Comparing `TorchRegister-0.2.0/src/TorchRegister/torchregister.py` & `TorchRegister-0.2.1/src/TorchRegister/torchregister.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         '''
         self.mode = mode
         self.warp = None if mode == 'flow' else get_affine_warp
         self.device = device
         self.debug = debug
         self.theta = None
 
-    def optim(self, moving, target, lr=1E-5, max_epochs=1000, n=16, per=0.1):
+    def optim(self, moving, target, lr=1E-5, max_epochs=1000, n=32, per=0.1):
         '''
         Optimization loop to get deformation matrix/flow-field
 
         Parameters
         ----------
         moving : tensor
             Tensor of shape [1,1,x,y,z] to be warped.
```

### Comparing `TorchRegister-0.2.0/src/TorchRegister/utils.py` & `TorchRegister-0.2.1/src/TorchRegister/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             self.reg[2].bias.data.copy_(torch.tensor(
                 [1, 0, 0, 0, 1, 0], dtype=torch.float))
         self.thetas = Theta()
 
     def forward(self, input_):
         var = self.reg(input_)
         theta = self.thetas(var)
-        if len(input_.shape) == 5:
+        if theta.shape[-1] == 12:
             return theta.view(1, 3, 4)
         else:
             return theta.view(1, 2, 3)
 
 
 class SpatialTransformer(nn.Module):
     '''
@@ -161,15 +161,15 @@
         y = self.bnorm(y)
         return y, w
 
 
 class Attention_UNet(nn.Module):
     def __init__(self, img_size, mode='nearest', in_c=1, n=1):
         super(Attention_UNet, self).__init__()
-        if len(img_size) == 5:
+        if len(img_size) == 3:
             out_c = 3
             self.layer1 = nn.Sequential(nn.Conv3d(in_channels=in_c, out_channels=int(64/n), kernel_size=3), nn.ReLU(), nn.InstanceNorm3d(int(64/n)),
                                         nn.Conv3d(in_channels=int(64/n), out_channels=int(64/n), kernel_size=3), nn.ReLU(), nn.InstanceNorm3d(int(64/n)))
 
             self.skip1 = attention_grid(
                 int(64/n), int(64/n), int(64/n), dims=3)
```

### Comparing `TorchRegister-0.2.0/src/TorchRegister/warpings.py` & `TorchRegister-0.2.1/src/TorchRegister/warpings.py`

 * *Files 16% similar despite different names*

```diff
@@ -109,23 +109,14 @@
                 plt.plot(losses_train, label='Error')
                 plt.title('Optimization Criterion')
                 plt.xlabel('Epoch')
                 plt.ylabel('Error')
                 plt.legend()
                 plt.show()
 
-                if len(moving.shape) == 5:
-                    plt.imshow(torch.squeeze(
-                        warped[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
-                else:
-                    plt.imshow(torch.squeeze(
-                        warped).detach().cpu().numpy(), cmap='gray')
-                plt.title('Warped Moving')
-                plt.show()
-
     regressor.eval()
     final_theta = regressor(input_)
     if len(moving.shape) == 5:
         final_theta = final_theta.view(1, 3, 4)
     else:
         final_theta = final_theta.view(1, 2, 3)
 
@@ -196,23 +187,14 @@
                 plt.plot(losses_train, label='Error')
                 plt.title('Optimization Criterion')
                 plt.xlabel('Epoch')
                 plt.ylabel('Error')
                 plt.legend()
                 plt.show()
 
-                if len(moving.shape) == 5:
-                    plt.imshow(torch.squeeze(
-                        warped[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
-                else:
-                    plt.imshow(torch.squeeze(
-                        warped).detach().cpu().numpy(), cmap='gray')
-                plt.title('Warped Moving')
-                plt.show()
-
     final_theta = regressor(input_)
     final_warped = get_affine_warp(final_theta, moving)
 
     return [final_warped, best_warped], [final_theta, best_theta]
 
 
 # Flow Registeration #
@@ -283,32 +265,14 @@
                     plt.plot(losses_train, label='Error')
                     plt.title('Optimization Criterion')
                     plt.xlabel('Epoch')
                     plt.ylabel('Error')
                     plt.legend()
                     plt.show()
 
-                    if len(moving.shape) == 5:
-                        plt.imshow(torch.squeeze(
-                            y[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
-                    else:
-                        plt.imshow(torch.squeeze(
-                            y).detach().cpu().numpy(), cmap='gray')
-                    plt.title('Warped Moving')
-                    plt.show()
-
-                    if len(moving.shape) == 5:
-                        plt.imshow(moveaxis(torch.squeeze(
-                            norm(torch.abs(self.flow[:, :, :, :, 60]))).detach().cpu().numpy(), 0, -1))
-                    else:
-                        plt.imshow(moveaxis(torch.squeeze(
-                            norm(torch.mean(torch.abs(self.flow), dim=1))).detach().cpu().numpy(), 0, -1), cmap='gray')
-                    plt.title('Flow Field')
-                    plt.show()
-
             if losses_train[-1] <= self.stop_crit:
                 message = 'Converged to %f' % self.stop_crit
                 break
 
         if debug:
             print('Optimization ended with status: %s' % message)
```

