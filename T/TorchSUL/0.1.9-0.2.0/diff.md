# Comparing `tmp/TorchSUL-0.1.9.tar.gz` & `tmp/TorchSUL-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TorchSUL-0.1.9.tar", last modified: Fri Feb 21 17:40:17 2020, max compression
+gzip compressed data, was "TorchSUL-0.2.0.tar", last modified: Sat Jul 15 09:50:20 2023, max compression
```

## Comparing `TorchSUL-0.1.9.tar` & `TorchSUL-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/
--rw-rw-rw-   0        0        0      405 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       83 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      559 2020-02-21 17:39:51.000000 TorchSUL-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/TorchSUL/
--rw-rw-rw-   0        0        0     3031 2020-02-06 08:20:11.000000 TorchSUL-0.1.9/TorchSUL/DataReader.py
--rw-rw-rw-   0        0        0    16629 2020-02-20 17:33:41.000000 TorchSUL-0.1.9/TorchSUL/Layers.py
--rw-rw-rw-   0        0        0     9515 2020-02-20 17:33:57.000000 TorchSUL-0.1.9/TorchSUL/Model.py
--rw-rw-rw-   0        0        0     1552 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/TorchSUL/sul_tool.py
--rw-rw-rw-   0        0        0      162 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/TorchSUL/__init__.py
-drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/TorchSUL.egg-info/
--rw-rw-rw-   0        0        0        1 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/top_level.txt
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.830544 TorchSUL-0.2.0/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3860 2023-07-15 09:50:20.828544 TorchSUL-0.2.0/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3621 2023-07-15 09:49:09.000000 TorchSUL-0.2.0/README.md
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.764228 TorchSUL-0.2.0/TorchSUL/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3859 2023-07-15 09:32:31.000000 TorchSUL-0.2.0/TorchSUL/Base.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-15 09:38:57.000000 TorchSUL-0.2.0/TorchSUL/Config.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22395 2023-07-15 08:51:32.000000 TorchSUL-0.2.0/TorchSUL/Layers.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    15107 2023-07-15 08:43:11.000000 TorchSUL-0.2.0/TorchSUL/Model.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13206 2023-07-07 15:01:14.000000 TorchSUL-0.2.0/TorchSUL/Quant.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.0/TorchSUL/__init__.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-15 08:15:48.000000 TorchSUL-0.2.0/TorchSUL/sul_tool.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-15 07:41:07.000000 TorchSUL-0.2.0/TorchSUL/sulplotter.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.816434 TorchSUL-0.2.0/TorchSUL.egg-info/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3860 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/requires.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/top_level.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-15 09:50:20.830544 TorchSUL-0.2.0/setup.cfg
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-15 08:14:28.000000 TorchSUL-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TorchSUL-0.1.9/TorchSUL/Layers.py` & `TorchSUL-0.2.0/TorchSUL/Layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,131 @@
+import functools
 import torch 
 import torch.nn as nn 
 import torch.nn.functional as F 
 import torch.nn.init as init 
 from torch.nn.parameter import Parameter
 import math 
-
-record_params = []
+import numpy as np 
+import torchvision.ops as ops
+from .Base import Model 
+from .Quant import QQuantizers, QObservers, QTYPES
 
 
 def _resnet_normal(tensor):
 	fan_in, fan_out = init._calculate_fan_in_and_fan_out(tensor)
 	std = math.sqrt(2.0 / float(fan_out))
 	return init._no_grad_normal_(tensor, 0., std)
 
-class Model(nn.Module):
-	def __init__(self, *args, **kwargs):
-		super(Model, self).__init__()
-		self.is_built = False
-		self.initialize(*args, **kwargs)
-
-	def initialize(self, *args, **kwargs):
-		pass 
-
-	def build(self, *inputs):
-		pass 
-
-	def __call__(self, *input, **kwargs):
-		if not self.is_built:
-			self.build(*input)
-		for hook in self._forward_pre_hooks.values():
-			result = hook(self, input)
-			if result is not None:
-				if not isinstance(result, tuple):
-					result = (result,)
-				input = result
-		if torch._C._get_tracing_state():
-			result = self._slow_forward(*input, **kwargs)
-		else:
-			result = self.forward(*input, **kwargs)
-		for hook in self._forward_hooks.values():
-			hook_result = hook(self, input, result)
-			if hook_result is not None:
-				result = hook_result
-		if len(self._backward_hooks) > 0:
-			var = result
-			while not isinstance(var, torch.Tensor):
-				if isinstance(var, dict):
-					var = next((v for v in var.values() if isinstance(v, torch.Tensor)))
-				else:
-					var = var[0]
-			grad_fn = var.grad_fn
-			if grad_fn is not None:
-				for hook in self._backward_hooks.values():
-					wrapper = functools.partial(hook, self)
-					functools.update_wrapper(wrapper, hook)
-					grad_fn.register_hook(wrapper)
-		self.is_built = True
-		return result
-
-	def record(self):
-		def set_record_flag(obj):
-			obj.record = True
-		self.apply(set_record_flag)
+######  Layers 
 
 class conv2D(Model):
 	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True, gropus=1):
 		self.size = size
 		self.outchn = outchn
 		self.stride = stride
 		self.usebias = usebias
 		self.gropus = gropus
 		self.dilation_rate = dilation_rate
 		assert (pad in ['VALID','SAME_LEFT'])
 		self.pad = pad 
 
 	def _parse_args(self, input_shape):
 		inchannel = input_shape[1]
+		self.inchannel = inchannel
 		# parse args
 		if isinstance(self.size,list):
-			# self.size = [self.size[0],self.size[1],inchannel,self.outchn]
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = ((self.size[0]+ (self.dilation_rate-1) * ( self.size-1 ))//2, (self.size[1]+ (self.dilation_rate-1) * ( self.size-1 ))//2)
 			self.size = [self.outchn, inchannel // self.gropus, self.size[0], self.size[1]]
 		else:
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2
 			self.size = [self.outchn, inchannel // self.gropus, self.size, self.size]
 
 	def build(self, *inputs):
-		# print('building...')
+		inp = inputs[0]
+		self._parse_args(inp.shape)
+		self.weight = Parameter(torch.Tensor(*self.size))
+		if self.usebias:
+			self.bias = Parameter(torch.Tensor(self.outchn))
+		else:
+			self.register_parameter('bias', None)
+		self.reset_params()
+
+		if self._quant:
+			bit_type = self.get_flag('QActBit')
+			if bit_type is None:
+				bit_type = 'int8'
+			obs_type = self.get_flag('QActObserver')
+			if obs_type is None:
+				obs_type = 'minmax'
+			self.input_quantizer = QQuantizers['uniform'](zero_offset=False, bit_type=bit_type, observer=obs_type)
+			self.w_quantizer = QQuantizers['uniform'](zero_offset=True, mode='channel_wise', is_weight=True)
+
+	def reset_params(self):
+		if self.get_flag('conv_init_mode')=='normal':
+			init.normal_(self.weight, std=0.001)
+		else:
+			_resnet_normal(self.weight)
+		if self.bias is not None:
+			if self.get_flag('conv_init_mode')=='normal':
+				init.zeros_(self.bias)
+			else:
+				fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
+				bound = 1 / math.sqrt(fan_in)
+				init.uniform_(self.bias, -bound, bound)
+
+	def forward(self, x):
+		weight = self.weight
+		if self._quant:
+			x = self.input_quantizer(x)
+			weight = self.w_quantizer(weight)
+		return F.conv2d(x, weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
+
+	def to_torch(self):
+		conv = nn.Conv2d(in_channels = self.inchannel, out_channels = self.outchn, kernel_size = tuple(self.size[2:]), stride = self.stride,\
+						padding = self.pad, padding_mode = 'zeros', dilation = self.dilation_rate, groups = self.gropus, bias = self.usebias)
+		conv.weight.data[:] = self.weight.data[:]
+		if self.usebias:
+			conv.bias.data[:] = self.bias.data[:]
+		return conv 
+
+
+class deconv2D(Model):
+	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True, gropus=1):
+		self.size = size
+		self.outchn = outchn
+		self.stride = stride
+		self.usebias = usebias
+		self.gropus = gropus
+		self.dilation_rate = dilation_rate
+		assert (pad in ['VALID','SAME_LEFT'])
+		self.pad = pad 
+		self.padmethod = pad
+
+	def _parse_args(self, input_shape):
+		inchannel = input_shape[1]
+		# parse args
+		if isinstance(self.size,int):
+			if self.pad == 'VALID':
+				self.pad = 0
+				self.out_pad = 0
+			else:
+				self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2 - (1 - self.size%2)
+				self.out_pad = self.stride - 1
+			self.size = [inchannel, self.outchn // self.gropus, self.size, self.size]
+		else:
+			raise Exception("Deconv kernel only supports int")
+
+	def build(self, *inputs):
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 		self.weight = Parameter(torch.Tensor(*self.size))
 		if self.usebias:
 			self.bias = Parameter(torch.Tensor(self.outchn))
 		else:
 			self.register_parameter('bias', None)
@@ -106,15 +135,22 @@
 		_resnet_normal(self.weight)
 		if self.bias is not None:
 			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
 			bound = 1 / math.sqrt(fan_in)
 			init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
-		return F.conv2d(x, self.weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
+		inh, inw = x.shape[2], x.shape[3]
+		x = F.conv_transpose2d(x, self.weight, self.bias, self.stride, self.pad, self.out_pad, self.gropus, self.dilation_rate)
+		outh, outw = x.shape[2], x.shape[3]
+		if self.padmethod=='SAME_LEFT':
+			if outh!=inh*self.stride or outw!=inw*self.stride:
+				x = x[:,:,:inh*self.stride,:inw*self.stride]
+		return x 
+
 
 class dwconv2D(Model):
 	# depth-wise conv2d
 	def initialize(self, size, multiplier, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True):
 		self.size = size
 		self.multiplier = multiplier
 		self.stride = stride
@@ -122,50 +158,59 @@
 		self.dilation_rate = dilation_rate
 		assert (pad in ['VALID','SAME_LEFT'])
 		self.pad = pad 
 
 	def _parse_args(self, input_shape):
 		inchannel = input_shape[1]
 		self.gropus = inchannel
+		self.inchannel = inchannel
+		self.outchn = self.multiplier * inchannel
 		# parse args
 		if isinstance(self.size,list):
-			# self.size = [self.size[0],self.size[1],inchannel,self.outchn]
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = ((self.size[0]+ (self.dilation_rate-1) * ( self.size-1 ))//2, (self.size[1]+ (self.dilation_rate-1) * ( self.size-1 ))//2)
 			self.size = [self.multiplier * inchannel, 1, self.size[0], self.size[1]]
 		else:
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2
 			self.size = [self.multiplier * inchannel, 1, self.size, self.size]
 
 	def build(self, *inputs):
-		# print('building...')
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 		self.weight = Parameter(torch.Tensor(*self.size))
 		if self.usebias:
-			self.bias = Parameter(torch.Tensor(self.outchn))
+			self.bias = Parameter(torch.Tensor(self.size[0]))
 		else:
 			self.register_parameter('bias', None)
 		self.reset_params()
 
 	def reset_params(self):
 		_resnet_normal(self.weight)
 		if self.bias is not None:
 			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
 			bound = 1 / math.sqrt(fan_in)
 			init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
 		return F.conv2d(x, self.weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
 
+	def to_torch(self):
+		conv = nn.Conv2d(in_channels = self.inchannel, out_channels = self.outchn, kernel_size = tuple(self.size[2:]), stride = self.stride,\
+						padding = self.pad, padding_mode = 'zeros', dilation = self.dilation_rate, groups = self.gropus, bias = self.usebias)
+		conv.weight.data[:] = self.weight.data[:]
+		if self.usebias:
+			conv.bias.data[:] = self.bias.data[:]
+		return conv 
+
+
 class conv1D(Model):
 	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True, gropus=1):
 		self.size = size
 		self.outchn = outchn
 		self.stride = stride
 		self.usebias = usebias
 		self.gropus = gropus
@@ -179,15 +224,14 @@
 		if self.pad == 'VALID':
 			self.pad = 0
 		else:
 			self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2
 		self.size = [self.outchn, inchannel // self.gropus, self.size]
 
 	def build(self, *inputs):
-		# print('building...')
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 		self.weight = Parameter(torch.Tensor(*self.size))
 		if self.usebias:
 			self.bias = Parameter(torch.Tensor(self.outchn))
 		else:
 			self.register_parameter('bias', None)
@@ -199,14 +243,15 @@
 			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
 			bound = 1 / math.sqrt(fan_in)
 			init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
 		return F.conv1d(x, self.weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
 
+
 class conv3D(Model):
 	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True, gropus=1):
 		self.size = size
 		self.outchn = outchn
 		self.stride = stride
 		self.usebias = usebias
 		self.gropus = gropus
@@ -214,29 +259,27 @@
 		assert (pad in ['VALID','SAME_LEFT'])
 		self.pad = pad 
 
 	def _parse_args(self, input_shape):
 		inchannel = input_shape[1]
 		# parse args
 		if isinstance(self.size,list) or isinstance(self.size, tuple):
-			# self.size = [self.size[0],self.size[1],inchannel,self.outchn]
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = ((self.size[0]+ (self.dilation_rate-1) * ( self.size-1 ))//2, (self.size[1]+ (self.dilation_rate-1) * ( self.size-1 ))//2, (self.size[2]+ (self.dilation_rate-1) * ( self.size-1 ))//2)
 			self.size = [self.outchn, inchannel // self.gropus, self.size[0], self.size[1], self.size[2]]
 		else:
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2
 			self.size = [self.outchn, inchannel // self.gropus, self.size, self.size, self.size]
 
 	def build(self, *inputs):
-		# print('building...')
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 		self.weight = Parameter(torch.Tensor(*self.size))
 		if self.usebias:
 			self.bias = Parameter(torch.Tensor(self.outchn))
 		else:
 			self.register_parameter('bias', None)
@@ -248,134 +291,127 @@
 			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
 			bound = 1 / math.sqrt(fan_in)
 			init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
 		return F.conv3d(x, self.weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
 
+
 class fclayer(Model):
 	def initialize(self, outsize, usebias=True, norm=False):
 		self.outsize = outsize
 		self.usebias = usebias
 		self.norm = norm
 
 	def build(self, *inputs):
-		# print('building...')
-		self.insize = inputs[0].shape[1]
+		self.insize = inputs[0].shape[-1]
 		self.weight = Parameter(torch.Tensor(self.outsize, self.insize))
 		if self.usebias:
 			self.bias = Parameter(torch.Tensor(self.outsize))
 		else:
 			self.register_parameter('bias', None)
 		self.reset_params()
 
 	def reset_params(self):
-		# init.kaiming_uniform_(self.weight, a=math.sqrt(5))
-		# init.normal_(self.weight, std=0.01)
-		_resnet_normal(self.weight)
-		print('Reset fc params...')
+		init.normal_(self.weight, std=0.001)
 		if self.bias is not None:
-			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
-			bound = 1 / math.sqrt(fan_in)
-			init.uniform_(self.bias, -bound, bound)
+			init.zeros_(self.bias)
 
 	def forward(self, x):
 		if self.norm:
 			with torch.no_grad():
 				norm = x.norm(p=2, dim=1, keepdim=True)
 				wnorm = self.weight.norm(p=2,dim=1, keepdim=True)
 			x = x / norm
 			weight = self.weight / wnorm
 		else:
 			weight = self.weight
 		return F.linear(x, weight, self.bias)
 
-def flatten(x):
-	x = x.view(x.size(0), -1)
-	return x 
+	def to_torch(self):
+		fc = nn.Linear(self.insize, self.outsize, self.usebias)
+		fc.weight.data[:] = self.weight.data[:]
+		if self.usebias:
+			fc.bias.data[:] = self.bias.data[:]
+		return fc 
 
-class Flatten(Model):
-	def forward(self, x):
-		return flatten(x)
 
 class MaxPool2d(Model):
 	def initialize(self, size, stride=1, pad='SAME_LEFT', dilation_rate=1):
 		self.size = size
 		self.stride = stride
 		self.pad = pad
 		self.dilation_rate = dilation_rate
 
 	def _parse_args(self, input_shape):
 		inchannel = input_shape[1]
 		# parse args
 		if isinstance(self.size,list) or isinstance(self.size, tuple):
-			# self.size = [self.size[0],self.size[1],inchannel,self.outchn]
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = (self.size[0]//2, self.size[1]//2, self.size[2]//2)
 		else:
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = self.size//2
 
 	def build(self, *inputs):
-		# print('building...')
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 
 	def forward(self, x):
 		return F.max_pool2d(x, self.size, self.stride, self.pad, self.dilation_rate, False, False)
 
+
 class AvgPool2d(Model):
 	def initialize(self, size, stride=1, pad='SAME_LEFT'):
 		self.size = size
 		self.stride = stride
 		self.pad = pad
 
 	def _parse_args(self, input_shape):
 		inchannel = input_shape[1]
 		# parse args
 		if isinstance(self.size,list) or isinstance(self.size, tuple):
-			# self.size = [self.size[0],self.size[1],inchannel,self.outchn]
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = (self.size[0]//2, self.size[1]//2, self.size[2]//2)
 		else:
 			if self.pad == 'VALID':
 				self.pad = 0
 			else:
 				self.pad = self.size//2
 
 	def build(self, *inputs):
-		# print('building...')
 		inp = inputs[0]
 		self._parse_args(inp.shape)
 
 	def forward(self, x):
 		return F.avg_pool2d(x, self.size, self.stride, self.pad, False, True)
 
+
 class BatchNorm(Model):
 	# _version = 2
 	# __constants__ = ['track_running_stats', 'momentum', 'eps', 'weight', 'bias',
 	# 				 'running_mean', 'running_var', 'num_batches_tracked',
 	# 				 'num_features', 'affine', 'weight', 'bias']
 
-	def initialize(self, eps=2e-5, momentum=0.01, affine=True,
+	def initialize(self, eps=None, momentum=0.01, affine=True,
 				 track_running_stats=True):
 		self.eps = eps
 		self.momentum = momentum
 		self.affine = affine
 		self.track_running_stats = track_running_stats
 		
 	def build(self, *inputs):
-		# print('building...')
 		num_features = inputs[0].shape[1]
+		self.num_features = num_features
 		if self.affine:
 			self.weight = Parameter(torch.Tensor(num_features))
 			self.bias = Parameter(torch.Tensor(num_features))
 		else:
 			self.register_parameter('weight', None)
 			self.register_parameter('bias', None)
 		if self.track_running_stats:
@@ -383,14 +419,16 @@
 			self.register_buffer('running_var', torch.ones(num_features))
 			self.register_buffer('num_batches_tracked', torch.tensor(0, dtype=torch.long))
 		else:
 			self.register_parameter('running_mean', None)
 			self.register_parameter('running_var', None)
 			self.register_parameter('num_batches_tracked', None)
 		self.reset_parameters()
+		eps = self.get_flag('bn_eps')
+		self.eps = 2e-5 if eps is None else eps 
 
 	def reset_running_stats(self):
 		if self.track_running_stats:
 			self.running_mean.zero_()
 			self.running_var.fill_(1)
 			self.num_batches_tracked.zero_()
 
@@ -417,14 +455,24 @@
 
 		result =  F.batch_norm(
 			input, self.running_mean, self.running_var, self.weight, self.bias,
 			self.training or not self.track_running_stats,
 			exponential_average_factor, self.eps)
 		return result
 
+	def to_torch(self):
+		bn = nn.BatchNorm2d(self.num_features, self.eps, self.momentum, self.affine, self.track_running_stats)
+		if self.affine:
+			bn.weight.data[:] = self.weight.data[:]
+			bn.bias.data[:] = self.bias.data[:]
+		if self.track_running_stats:
+			bn.running_mean.data[:] = self.running_mean.data[:]
+			bn.running_var.data[:] = self.running_var.data[:]
+		return bn 
+
 	# def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict,
 	# 						  missing_keys, unexpected_keys, error_msgs):
 	# 	version = local_metadata.get('version', None)
 
 	# 	if (version is None or version < 2) and self.track_running_stats:
 	# 		# at version 2: added num_batches_tracked buffer
 	# 		#			   this should have a default value of 0
@@ -432,58 +480,105 @@
 	# 		if num_batches_tracked_key not in state_dict:
 	# 			state_dict[num_batches_tracked_key] = torch.tensor(0, dtype=torch.long)
 
 	# 	super(_BatchNorm, self)._load_from_state_dict(
 	# 		state_dict, prefix, local_metadata, strict,
 	# 		missing_keys, unexpected_keys, error_msgs)
 
-def GlobalAvgPool2D(x):
-	x = x.mean(dim=(2,3), keepdim=True)
-	return x 
 
-class GlobalAvgPool2DLayer(Model):
+class LayerNorm(Model):
+	def initialize(self, n_dims_to_keep, affine=True, eps=1e-5):
+		self.n_dims_to_keep = n_dims_to_keep
+		self.affine = affine
+		self.eps = eps 
+
+	def build(self, *inputs):
+		shape = inputs[0].shape
+		n_dims = len(shape)
+		self.dim_to_reduce = tuple(range(n_dims - self.n_dims_to_keep, n_dims))
+		if self.affine:
+			self.weight = Parameter(torch.Tensor(*shape[-self.n_dims_to_keep:]))
+			self.bias = Parameter(torch.Tensor(*shape[-self.n_dims_to_keep:]))
+		self.reset_params()
+
+	def reset_params(self):
+		if self.affine:
+			init.ones_(self.weight)
+			init.zeros_(self.bias)
+
+	def forward(self, x):
+		mean = torch.mean(x, dim=self.dim_to_reduce, keepdim=True)
+		std = torch.std(x, dim=self.dim_to_reduce, keepdim=True)
+		if self.affine:
+			return self.weight * (x - mean) / (std + self.eps) + self.bias
+		else:
+			return (x - mean) / (std + self.eps)
+
+
+class NNUpSample(Model):
+	def initialize(self, scale):
+		self.scale = scale
+
+	def _parse_args(self, input_shape):
+		self.inchannel = input_shape[1]
+		self.size = [self.inchannel, 1, self.scale, self.scale]
+
+	def build(self, *inputs):
+		inp = inputs[0]
+		self._parse_args(inp.shape)
+		self.weight = Parameter(torch.Tensor(*self.size), requires_grad=False)
+		self.register_parameter('bias', None)
+		self.reset_params()
+
+	def reset_params(self):
+		init.ones_(self.weight)
+
 	def forward(self, x):
-		return GlobalAvgPool2D(x)
+		# w = self.weight.detach()
+		w = self.weight
+		return F.conv_transpose2d(x, w, self.bias, self.scale, 0, 0, self.inchannel, 1)
+
 
 def activation(x, act, **kwargs):
 	if act==-1:
 		return x
 	elif act==0:
 		return F.relu(x)
 	elif act==1:
-		return F.leaky_relu(x, negative_slope=0.2)
+		return F.leaky_relu(x, negative_slope=0.1)
 	elif act==2:
 		return F.elu(x)
 	elif act==3:
 		return F.tanh(x)
 	elif act==6:
 		return torch.sigmoid(x)
+	elif act==10:
+		return F.gelu(x)
+
 
 class Activation(Model):
 	def initialize(self, act):
 		self.act = act 
 		if act==8:
-			self.act = torch.nn.PReLU(num_parameters=outchn)
+			self.act = torch.nn.PReLU(num_parameters=outchn)  # this line is buggy
 		elif act==9:
 			self.act = torch.nn.PReLU(num_parameters=1)
+
 	def forward(self, x):
 		if self.act==8 or self.act==9:
 			return self.act(x)
 		else:
 			return activation(x, self.act)
 
+
 class graphConvLayer(Model):
-	def __init__(self, outsize, adj_mtx=None, adj_fn=None, values=None, usebias=True):
-		assert (adj_mtx is None) ^ (adj_fn is None), 'Assign either adj_mtx or adj_fn' 
+	def initialize(self, outsize, usebias=True, norm=True):
 		self.outsize = outsize
-		self.adj_mtx = adj_mtx
-		self.adj_fn = adj_fn
-		self.values = values
 		self.usebias = usebias
-		self.normalized = False
+		self.norm = norm 
 
 	def _parse_args(self, input_shape):
 		# set size
 		insize = input_shape[-1]
 		self.size = [self.outsize, insize]
 
 	def build(self, *inputs):
@@ -511,19 +606,101 @@
 			S = torch.diag(S)
 			I = torch.eye(S.shape[0])
 			A_ = (mtx + I) 
 			A_ = torch.mm(S, A_)
 			A_ = torch.mm(A_, S)
 		return A_
 
-	def forward(self, x):
-		if self.adj_mtx is not None:
-			if not self.normalized:
-				self.adj_mtx = self._normalize_adj_mtx(self.adj_mtx)
-				self.normalized = True
-		else:
-			A = self.adj_fn(x)
-		res = torch.mm(A, x)
+	def forward(self, x, adj, affinity_grad=True):
+		if self.norm:
+			adj = self._normalize_adj_mtx(adj)
+		if not affinity_grad:
+			adj = adj.detach()
+		res = torch.mm(adj, x)
 		res = F.linear(res, self.weight, self.bias)
 		return res 
 	
 
+class BilinearUpSample(Model):
+	def initialize(self, factor):
+		self.factor = factor
+		self.pad0 = factor//2 * 3 + factor%2
+
+	def build(self, *inputs):
+		inp = inputs[0]
+		self.inchn = inp.shape[1]
+		filter_size = 2*self.factor - self.factor%2
+		k = self.upsample_kernel(filter_size)
+		k = k[None, ...]
+		k = k[None, ...]
+		k = np.repeat(k, self.inchn, axis=0)
+		self.weight = Parameter(torch.from_numpy(k), requires_grad=False)
+
+	def upsample_kernel(self,size):
+		factor = (size +1)//2
+		if size%2==1:
+			center = factor - 1
+		else:
+			center = factor - 0.5
+		og = np.ogrid[:size, :size]
+		k = (1 - abs(og[0]-center)/factor) * (1-abs(og[1]-center)/factor)
+		return np.float32(k)
+
+	def forward(self, x):
+		x = F.pad(x, (1,1,1,1), 'replicate')
+		x = F.conv_transpose2d(x, self.weight, None, self.factor, self.pad0, 0, self.inchn, 1)
+		return x 
+
+	def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs):
+		pass
+
+	def _save_to_state_dict(self, destination, prefix, keep_vars):
+		pass
+
+
+class DeformConv2D(Model):
+	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, usebias=True):
+		self.size = size
+		self.outchn = outchn
+		self.stride = stride
+		self.usebias = usebias
+		self.dilation_rate = dilation_rate
+		assert (pad in ['VALID','SAME_LEFT'])
+		self.pad = pad 
+
+	def _parse_args(self, input_shape):
+		inchannel = input_shape[1]
+		self.inchannel = inchannel
+		# parse args
+		if isinstance(self.size,list):
+			if self.pad == 'VALID':
+				self.pad = 0
+			else:
+				self.pad = ((self.size[0]+ (self.dilation_rate-1) * ( self.size-1 ))//2, (self.size[1]+ (self.dilation_rate-1) * ( self.size-1 ))//2)
+			self.size = [self.outchn, inchannel, self.size[0], self.size[1]]
+		else:
+			if self.pad == 'VALID':
+				self.pad = 0
+			else:
+				self.pad = (self.size + (self.dilation_rate-1) * ( self.size-1 ))//2
+			self.size = [self.outchn, inchannel, self.size, self.size]
+
+	def build(self, *inputs):
+		inp = inputs[0]
+		self._parse_args(inp.shape)
+		self.weight = Parameter(torch.Tensor(*self.size))
+		if self.usebias:
+			self.bias = Parameter(torch.Tensor(self.outchn))
+		else:
+			self.register_parameter('bias', None)
+		self.reset_params()
+
+	def reset_params(self):
+		_resnet_normal(self.weight)
+		if self.bias is not None:
+			fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
+			bound = 1 / math.sqrt(fan_in)
+			init.uniform_(self.bias, -bound, bound)
+
+	def forward(self, x, offset):
+		return ops.deform_conv2d(x, offset, self.weight, self.bias, self.stride, self.pad, self.dilation_rate)
+
```

