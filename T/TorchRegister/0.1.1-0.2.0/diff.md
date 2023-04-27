# Comparing `tmp/TorchRegister-0.1.1.tar.gz` & `tmp/TorchRegister-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchRegister-0.1.1.tar", last modified: Tue Apr 18 01:22:15 2023, max compression
+gzip compressed data, was "TorchRegister-0.2.0.tar", last modified: Thu Apr 27 22:32:41 2023, max compression
```

## Comparing `TorchRegister-0.1.1.tar` & `TorchRegister-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:22:15.627661 TorchRegister-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 01:22:15.627661 TorchRegister-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:22:15.627661 TorchRegister-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:22:15.623660 TorchRegister-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:22:15.623660 TorchRegister-0.1.1/src/TorchRegister/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/src/TorchRegister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/src/TorchRegister/torchregister.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/src/TorchRegister/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-18 01:22:00.000000 TorchRegister-0.1.1/src/TorchRegister/warpings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:22:15.627661 TorchRegister-0.1.1/src/TorchRegister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 01:22:15.000000 TorchRegister-0.1.1/src/TorchRegister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 01:22:15.000000 TorchRegister-0.1.1/src/TorchRegister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:22:15.000000 TorchRegister-0.1.1/src/TorchRegister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 01:22:15.000000 TorchRegister-0.1.1/src/TorchRegister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 01:22:15.000000 TorchRegister-0.1.1/src/TorchRegister.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.714936 TorchRegister-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.714936 TorchRegister-0.2.0/src/TorchRegister/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/torchregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15689 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-04-27 22:32:28.000000 TorchRegister-0.2.0/src/TorchRegister/warpings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:32:41.718936 TorchRegister-0.2.0/src/TorchRegister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 22:32:41.000000 TorchRegister-0.2.0/src/TorchRegister.egg-info/top_level.txt
```

### Comparing `TorchRegister-0.1.1/LICENSE.md` & `TorchRegister-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.1.1/README.md` & `TorchRegister-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 <p>Example:</p>
  <pre><code>
  
         import torch
         from torchio.transforms import RandomAffine
         from numpy import load
         from matplotlib import pyplot as plt
-        from torchregister import Register
+        from TorchRegister import Register
 
 
         # augmentation function
         def rand_augment(x):
             affine = RandomAffine(image_interpolation='bspline',
                                   degrees=45, translation=8, scales=(0.7, 1.5))
             y = affine(x[0])
@@ -33,17 +33,20 @@
 
 
         device = 'cuda'
 
         # loading data
         path = 'example_mri.pkl'
         data = load(path, allow_pickle=True)
+        
+        moving = torch.from_numpy(data)
         moving = moving.view(1, 1, moving.shape[0], moving.shape[1], moving.shape[2]).to(
             dtype=torch.float, device=device)
-        target = torch.from_numpy(data[0])
+        
+        target = torch.from_numpy(data)
         target = rand_augment(target.view(1, 1, target.shape[0], target.shape[1], target.shape[2])).to(
             dtype=torch.float, device=device)
 
         # Flow field based registration
         warping = Register(mode='flow', device=device, debug=True)
         warping.optim(moving, target, lr=1E-3)
         warped = warping(moving)
```

### Comparing `TorchRegister-0.1.1/setup.py` & `TorchRegister-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TorchRegister',
-    version='0.1.1',
+    version='0.2.0',
     url='https://github.com/AgamChopra/TorchRegister',
     author='Agam Chopra',
     author_email='achopra4@uw.edu',
     description='3D image registration methods for PyTorch.',
     long_description='Common medical 3D image registration methods such as rigid, affine, and flow field for PyTorch.',
     install_requires=['torch >= 2.0.0', 'numpy >= 1.24.1',
                       'tqdm >= 4.65.0', 'matplotlib  >= 3.7.1'],
```

### Comparing `TorchRegister-0.1.1/src/TorchRegister/torchregister.py` & `TorchRegister-0.2.0/src/TorchRegister/torchregister.py`

 * *Files identical despite different names*

### Comparing `TorchRegister-0.1.1/src/TorchRegister/warpings.py` & `TorchRegister-0.2.0/src/TorchRegister/warpings.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,38 +13,60 @@
 from matplotlib import pyplot as plt
 
 from .utils import Regressor, Attention_UNet, norm
 
 
 # Warping Function #
 def get_affine_warp(theta, moving):
+    if len(theta.shape) == 2:
+        if theta.shape[-1] == 6:
+            theta = theta.view(1, 2, 3)
+        else:
+            theta = theta.view(1, 3, 4)
     grid = F.affine_grid(theta, moving.size(), align_corners=False)
     warped = F.grid_sample(moving, grid, align_corners=False, mode='bilinear')
     return warped
 
 
 # Affine Registration #
-def affine_register(moving, target, lr=1E-5, epochs=1000, per=0.1, device='cpu', debug=True):
+def affine_register(moving, target, lr=1E-5, epochs=1000, per=0.1, device='cpu', debug=True, idx=60):
     if debug:
-        plt.imshow(torch.squeeze(
-            moving[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+        if len(moving.shape) == 5:
+            plt.imshow(torch.squeeze(
+                moving[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+        else:
+            plt.imshow(torch.squeeze(
+                moving).detach().cpu().numpy(), cmap='gray')
         plt.title('Moving')
         plt.show()
 
-        plt.imshow(torch.squeeze(
-            target[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+        if len(moving.shape) == 5:
+            plt.imshow(torch.squeeze(
+                target[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+        else:
+            plt.imshow(torch.squeeze(
+                target).detach().cpu().numpy(), cmap='gray')
         plt.title('Target')
         plt.show()
 
-    regressor = nn.Sequential(nn.Linear(int(2 * per * (torch.flatten(
-        moving).shape[0])), 64, bias=False), nn.ReLU(), nn.Linear(64, 12)).to(device=device)
-    regressor[0].weight.data.zero_()
-    regressor[2].weight.data.zero_()
-    regressor[2].bias.data.copy_(torch.tensor(
-        [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0], dtype=torch.float))
+    if len(moving.shape) == 5:
+        regressor = nn.Sequential(nn.Linear(int(2 * per * (torch.flatten(
+            moving).shape[0])), 64, bias=False), nn.ReLU(), nn.Linear(64, 12)).to(device=device)
+        regressor[0].weight.data.zero_()
+        regressor[2].weight.data.zero_()
+        regressor[2].bias.data.copy_(torch.tensor(
+            [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0], dtype=torch.float))
+    else:
+        regressor = nn.Sequential(nn.Linear(int(2 * per * (torch.flatten(
+            moving).shape[0])), 32, bias=False), nn.ReLU(), nn.Linear(32, 6)).to(device=device)
+        regressor[0].weight.data.zero_()
+        regressor[2].weight.data.zero_()
+        regressor[2].bias.data.copy_(torch.tensor(
+            [1, 0, 0, 0, 1, 0], dtype=torch.float))
+
     params = regressor.parameters()
     optimizer = torch.optim.SGD(params, lr)
     criterions = [nn.MSELoss(), nn.L1Loss()]
     weights = [0.5, 0.5]
 
     regressor.train()
     losses_train = []
@@ -53,15 +75,20 @@
         moving).shape[-1]), int(per * torch.flatten(moving).shape[0]))
     input_ = torch.cat((torch.flatten(moving).view(
         1, -1)[:, idx], torch.flatten(target).view(1, -1)[:, idx]), dim=1)
 
     for eps in trange(epochs):
         optimizer.zero_grad()
 
-        theta = regressor(input_).view(1, 3, 4)  # 3D Affine Matrix
+        theta = regressor(input_)  # 3D Affine Matrix
+        if len(moving.shape) == 5:
+            theta = theta.view(1, 3, 4)
+        else:
+            theta = theta.view(1, 2, 3)
+
         warped = get_affine_warp(theta, moving)
 
         error = sum([weights[i] * criterions[i](target, warped)
                     for i in range(len(criterions))])
         error.backward()
         optimizer.step()
 
@@ -82,36 +109,53 @@
                 plt.plot(losses_train, label='Error')
                 plt.title('Optimization Criterion')
                 plt.xlabel('Epoch')
                 plt.ylabel('Error')
                 plt.legend()
                 plt.show()
 
-                plt.imshow(torch.squeeze(
-                    warped[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+                if len(moving.shape) == 5:
+                    plt.imshow(torch.squeeze(
+                        warped[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+                else:
+                    plt.imshow(torch.squeeze(
+                        warped).detach().cpu().numpy(), cmap='gray')
                 plt.title('Warped Moving')
                 plt.show()
 
     regressor.eval()
-    final_theta = regressor(input_).view(1, 3, 4)
+    final_theta = regressor(input_)
+    if len(moving.shape) == 5:
+        final_theta = final_theta.view(1, 3, 4)
+    else:
+        final_theta = final_theta.view(1, 2, 3)
+
     final_warped = get_affine_warp(final_theta, moving)
 
     return [final_warped, best_warped], [final_theta, best_theta]
 
 
 # Rigid Registration #
-def rigid_register(moving, target, lr=1E-5, epochs=1000, per=0.1, device='cpu', debug=True):
+def rigid_register(moving, target, lr=1E-5, epochs=1000, per=0.1, device='cpu', debug=True, idx=60):
     if debug:
-        plt.imshow(torch.squeeze(
-            moving[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+        if len(moving.shape) == 5:
+            plt.imshow(torch.squeeze(
+                moving[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+        else:
+            plt.imshow(torch.squeeze(
+                moving).detach().cpu().numpy(), cmap='gray')
         plt.title('Moving')
         plt.show()
 
-        plt.imshow(torch.squeeze(
-            target[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+        if len(moving.shape) == 5:
+            plt.imshow(torch.squeeze(
+                target[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+        else:
+            plt.imshow(torch.squeeze(
+                target).detach().cpu().numpy(), cmap='gray')
         plt.title('Target')
         plt.show()
 
     regressor = Regressor(moving, per, device)
     params = regressor.parameters()
     optimizer = torch.optim.SGD(params, lr)
     criterions = [nn.MSELoss(), nn.L1Loss()]
@@ -152,16 +196,20 @@
                 plt.plot(losses_train, label='Error')
                 plt.title('Optimization Criterion')
                 plt.xlabel('Epoch')
                 plt.ylabel('Error')
                 plt.legend()
                 plt.show()
 
-                plt.imshow(torch.squeeze(
-                    warped[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+                if len(moving.shape) == 5:
+                    plt.imshow(torch.squeeze(
+                        warped[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+                else:
+                    plt.imshow(torch.squeeze(
+                        warped).detach().cpu().numpy(), cmap='gray')
                 plt.title('Warped Moving')
                 plt.show()
 
     final_theta = regressor(input_)
     final_warped = get_affine_warp(final_theta, moving)
 
     return [final_warped, best_warped], [final_theta, best_theta]
@@ -169,18 +217,18 @@
 
 # Flow Registeration #
 class flow_register(nn.Module):
     '''
     Non-linear model for 3D image registration via overfitting.
     '''
 
-    def __init__(self, img_size, mode='bilinear', in_c=1, out_c=3, n=1, criterions=[nn.MSELoss(), nn.L1Loss()], weights=[0.5, 0.5], lr=1E-3, max_epochs=2000, stop_crit=1E-4):
+    def __init__(self, img_size, mode='bilinear', in_c=1, n=1, criterions=[nn.MSELoss(), nn.L1Loss()], weights=[0.5, 0.5], lr=1E-3, max_epochs=2000, stop_crit=1E-4):
         super(flow_register, self).__init__()
         self.model = Attention_UNet(
-            img_size, mode, in_c=in_c, out_c=out_c, n=n)
+            img_size, mode, in_c=in_c, n=n)
 
         self.flow = None
 
         self.warp = None
 
         self.criterions, self.weights, self.lr, self.max_epochs, self.stop_crit = criterions, weights, lr, max_epochs, stop_crit
 
@@ -188,27 +236,35 @@
 
         self.optimizer = torch.optim.Adam(params, self.lr)
 
     def forward(self, x, device):
         y, self.flow = self.model(x, device)
         return y
 
-    def optimize(self, moving, target, device, debug=True):
+    def optimize(self, moving, target, device, debug=True, idx=60):
         losses_train = []
         message = 'Reached max epochs'
         self.train()
 
         if debug:
-            plt.imshow(torch.squeeze(
-                moving[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+            if len(moving.shape) == 5:
+                plt.imshow(torch.squeeze(
+                    moving[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+            else:
+                plt.imshow(torch.squeeze(
+                    moving).detach().cpu().numpy(), cmap='gray')
             plt.title('Moving')
             plt.show()
 
-            plt.imshow(torch.squeeze(
-                target[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+            if len(moving.shape) == 5:
+                plt.imshow(torch.squeeze(
+                    target[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+            else:
+                plt.imshow(torch.squeeze(
+                    target).detach().cpu().numpy(), cmap='gray')
             plt.title('Target')
             plt.show()
 
         for eps in trange(self.max_epochs):
             self.optimizer.zero_grad()
 
             y = self(moving, device)
@@ -227,21 +283,29 @@
                     plt.plot(losses_train, label='Error')
                     plt.title('Optimization Criterion')
                     plt.xlabel('Epoch')
                     plt.ylabel('Error')
                     plt.legend()
                     plt.show()
 
-                    plt.imshow(torch.squeeze(
-                        y[:, :, :, :, 60]).detach().cpu().numpy(), cmap='gray')
+                    if len(moving.shape) == 5:
+                        plt.imshow(torch.squeeze(
+                            y[:, :, :, :, idx]).detach().cpu().numpy(), cmap='gray')
+                    else:
+                        plt.imshow(torch.squeeze(
+                            y).detach().cpu().numpy(), cmap='gray')
                     plt.title('Warped Moving')
                     plt.show()
 
-                    plt.imshow(moveaxis(torch.squeeze(
-                        norm(torch.abs(self.flow[:, :, :, :, 60]))).detach().cpu().numpy(), 0, -1))
+                    if len(moving.shape) == 5:
+                        plt.imshow(moveaxis(torch.squeeze(
+                            norm(torch.abs(self.flow[:, :, :, :, 60]))).detach().cpu().numpy(), 0, -1))
+                    else:
+                        plt.imshow(moveaxis(torch.squeeze(
+                            norm(torch.mean(torch.abs(self.flow), dim=1))).detach().cpu().numpy(), 0, -1), cmap='gray')
                     plt.title('Flow Field')
                     plt.show()
 
             if losses_train[-1] <= self.stop_crit:
                 message = 'Converged to %f' % self.stop_crit
                 break
```

