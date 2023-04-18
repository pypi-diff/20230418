# Comparing `tmp/lossers-0.0.2.tar.gz` & `tmp/lossers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.2.tar", last modified: Sun Apr 16 02:50:07 2023, max compression
+gzip compressed data, was "lossers-0.0.3.tar", last modified: Tue Apr 18 11:41:24 2023, max compression
```

## Comparing `lossers-0.0.2.tar` & `lossers-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.597660 lossers-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-03-24 10:25:10.000000 lossers-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      543 2023-04-16 02:50:07.597660 lossers-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-04-15 09:30:19.000000 lossers-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.577660 lossers-0.0.2/lossers/
--rw-rw-rw-   0        0        0        0 2023-04-15 09:04:19.000000 lossers-0.0.2/lossers/__init__.py
--rw-rw-rw-   0        0        0      436 2023-04-15 09:27:11.000000 lossers-0.0.2/lossers/clip.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.597660 lossers-0.0.2/lossers/lpips/
--rw-rw-rw-   0        0        0       26 2023-04-16 02:21:05.000000 lossers-0.0.2/lossers/lpips/__init__.py
--rw-rw-rw-   0        0        0     4211 2023-04-16 02:41:50.000000 lossers-0.0.2/lossers/lpips/lpips.py
--rw-rw-rw-   0        0        0     3128 2023-04-16 01:02:20.000000 lossers-0.0.2/lossers/lpips/pretrained_model.py
--rw-rw-rw-   0        0        0     2776 2023-04-15 09:13:24.000000 lossers-0.0.2/lossers/ssim.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.587665 lossers-0.0.2/lossers.egg-info/
--rw-rw-rw-   0        0        0      543 2023-04-16 02:50:06.000000 lossers-0.0.2/lossers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 02:50:07.597660 lossers-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-16 02:44:21.000000 lossers-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 11:41:13.000000 lossers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 11:41:24.337189 lossers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 11:41:13.000000 lossers-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers/lpips/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:41:24.337189 lossers-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 11:41:13.000000 lossers-0.0.3/setup.py
```

### Comparing `lossers-0.0.2/LICENSE` & `lossers-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mr. Zhang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mr. Zhang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `lossers-0.0.2/PKG-INFO` & `lossers-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: lossers
-Version: 0.0.2
-Summary: ML Loss Function
-Home-page: https://github.com/JiauZhang/lossers
-Author: JiauZhang
-Author-email: jiauzhang@163.com
-License: MIT
-Keywords: artificial intelligence,loss function,deep learning
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: lossers
+Version: 0.0.3
+Summary: ML Loss Function
+Home-page: https://github.com/JiauZhang/lossers
+Author: JiauZhang
+Author-email: jiauzhang@163.com
+License: MIT
+Keywords: artificial intelligence,loss function,deep learning
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `lossers-0.0.2/lossers/ssim.py` & `lossers-0.0.3/lossers/ssim.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import torch
-import torch.nn.functional as F
-from torch.autograd import Variable
-from math import exp
-
-# from https://github.com/Po-Hsun-Su/pytorch-ssim/blob/master/pytorch_ssim/__init__.py
-def gaussian(window_size, sigma):
-    gauss = torch.Tensor([exp(-(x - window_size//2)**2/float(2*sigma**2)) for x in range(window_size)])
-    return gauss/gauss.sum()
-
-def create_window(window_size, channel):
-    _1D_window = gaussian(window_size, 1.5).unsqueeze(1)
-    _2D_window = _1D_window.mm(_1D_window.t()).float().unsqueeze(0).unsqueeze(0)
-    window = Variable(_2D_window.expand(channel, 1, window_size, window_size).contiguous())
-    return window
-
-def _ssim(img1, img2, window, window_size, channel, size_average = True):
-    mu1 = F.conv2d(img1, window, padding = window_size//2, groups = channel)
-    mu2 = F.conv2d(img2, window, padding = window_size//2, groups = channel)
-
-    mu1_sq = mu1.pow(2)
-    mu2_sq = mu2.pow(2)
-    mu1_mu2 = mu1*mu2
-
-    sigma1_sq = F.conv2d(img1*img1, window, padding = window_size//2, groups = channel) - mu1_sq
-    sigma2_sq = F.conv2d(img2*img2, window, padding = window_size//2, groups = channel) - mu2_sq
-    sigma12 = F.conv2d(img1*img2, window, padding = window_size//2, groups = channel) - mu1_mu2
-
-    C1 = 0.01**2
-    C2 = 0.03**2
-
-    ssim_map = ((2*mu1_mu2 + C1)*(2*sigma12 + C2))/((mu1_sq + mu2_sq + C1)*(sigma1_sq + sigma2_sq + C2))
-
-    if size_average:
-        return ssim_map.mean()
-    else:
-        return ssim_map.mean(1).mean(1).mean(1)
-
-class SSIM(torch.nn.Module):
-    def __init__(self, window_size = 11, size_average = True):
-        super(SSIM, self).__init__()
-        self.window_size = window_size
-        self.size_average = size_average
-        self.channel = 1
-        self.window = create_window(window_size, self.channel)
-
-    def forward(self, img1, img2):
-        (_, channel, _, _) = img1.size()
-
-        if channel == self.channel and self.window.data.type() == img1.data.type():
-            window = self.window
-        else:
-            window = create_window(self.window_size, channel)
-            
-            if img1.is_cuda:
-                window = window.cuda(img1.get_device())
-            window = window.type_as(img1)
-            
-            self.window = window
-            self.channel = channel
-
-
-        return _ssim(img1, img2, window, self.window_size, channel, self.size_average)
-
-def ssim(img1, img2, window_size = 11, size_average = True):
-    (_, channel, _, _) = img1.size()
-    window = create_window(window_size, channel)
-    
-    if img1.is_cuda:
-        window = window.cuda(img1.get_device())
-    window = window.type_as(img1)
-    
-    return _ssim(img1, img2, window, window_size, channel, size_average)
+import torch
+import torch.nn.functional as F
+from torch.autograd import Variable
+from math import exp
+
+# from https://github.com/Po-Hsun-Su/pytorch-ssim/blob/master/pytorch_ssim/__init__.py
+def gaussian(window_size, sigma):
+    gauss = torch.Tensor([exp(-(x - window_size//2)**2/float(2*sigma**2)) for x in range(window_size)])
+    return gauss/gauss.sum()
+
+def create_window(window_size, channel):
+    _1D_window = gaussian(window_size, 1.5).unsqueeze(1)
+    _2D_window = _1D_window.mm(_1D_window.t()).float().unsqueeze(0).unsqueeze(0)
+    window = Variable(_2D_window.expand(channel, 1, window_size, window_size).contiguous())
+    return window
+
+def _ssim(img1, img2, window, window_size, channel, size_average = True):
+    mu1 = F.conv2d(img1, window, padding = window_size//2, groups = channel)
+    mu2 = F.conv2d(img2, window, padding = window_size//2, groups = channel)
+
+    mu1_sq = mu1.pow(2)
+    mu2_sq = mu2.pow(2)
+    mu1_mu2 = mu1*mu2
+
+    sigma1_sq = F.conv2d(img1*img1, window, padding = window_size//2, groups = channel) - mu1_sq
+    sigma2_sq = F.conv2d(img2*img2, window, padding = window_size//2, groups = channel) - mu2_sq
+    sigma12 = F.conv2d(img1*img2, window, padding = window_size//2, groups = channel) - mu1_mu2
+
+    C1 = 0.01**2
+    C2 = 0.03**2
+
+    ssim_map = ((2*mu1_mu2 + C1)*(2*sigma12 + C2))/((mu1_sq + mu2_sq + C1)*(sigma1_sq + sigma2_sq + C2))
+
+    if size_average:
+        return ssim_map.mean()
+    else:
+        return ssim_map.mean(1).mean(1).mean(1)
+
+class SSIM(torch.nn.Module):
+    def __init__(self, window_size = 11, size_average = True):
+        super(SSIM, self).__init__()
+        self.window_size = window_size
+        self.size_average = size_average
+        self.channel = 1
+        self.window = create_window(window_size, self.channel)
+
+    def forward(self, img1, img2):
+        (_, channel, _, _) = img1.size()
+
+        if channel == self.channel and self.window.data.type() == img1.data.type():
+            window = self.window
+        else:
+            window = create_window(self.window_size, channel)
+            
+            if img1.is_cuda:
+                window = window.cuda(img1.get_device())
+            window = window.type_as(img1)
+            
+            self.window = window
+            self.channel = channel
+
+
+        return _ssim(img1, img2, window, self.window_size, channel, self.size_average)
+
+def ssim(img1, img2, window_size = 11, size_average = True):
+    (_, channel, _, _) = img1.size()
+    window = create_window(window_size, channel)
+    
+    if img1.is_cuda:
+        window = window.cuda(img1.get_device())
+    window = window.type_as(img1)
+    
+    return _ssim(img1, img2, window, window_size, channel, size_average)
```

### Comparing `lossers-0.0.2/lossers.egg-info/PKG-INFO` & `lossers-0.0.3/lossers.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: lossers
-Version: 0.0.2
-Summary: ML Loss Function
-Home-page: https://github.com/JiauZhang/lossers
-Author: JiauZhang
-Author-email: jiauzhang@163.com
-License: MIT
-Keywords: artificial intelligence,loss function,deep learning
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: lossers
+Version: 0.0.3
+Summary: ML Loss Function
+Home-page: https://github.com/JiauZhang/lossers
+Author: JiauZhang
+Author-email: jiauzhang@163.com
+License: MIT
+Keywords: artificial intelligence,loss function,deep learning
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

