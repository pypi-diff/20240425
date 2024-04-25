# Comparing `tmp/bert4keras3-1.2.9-py3-none-any.whl.zip` & `tmp/bert4keras3-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 59695 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      150 b- defN 24-Mar-27 11:41 bert4keras3/__init__.py
--rw-rw-rw-  2.0 fat    20229 b- defN 24-Mar-27 11:41 bert4keras3/backend.py
--rw-rw-rw-  2.0 fat    52459 b- defN 24-Mar-27 14:03 bert4keras3/layers.py
--rw-rw-rw-  2.0 fat   124407 b- defN 24-Apr-17 09:24 bert4keras3/models.py
--rw-rw-rw-  2.0 fat    30152 b- defN 24-Mar-27 11:41 bert4keras3/ops.py
--rw-rw-rw-  2.0 fat    27955 b- defN 24-Mar-27 11:41 bert4keras3/snippets.py
--rw-rw-rw-  2.0 fat    15509 b- defN 24-Mar-27 11:41 bert4keras3/tokenizers.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-17 09:25 bert4keras3-1.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      221 b- defN 24-Apr-17 09:25 bert4keras3-1.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 09:25 bert4keras3-1.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-17 09:25 bert4keras3-1.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      964 b- defN 24-Apr-17 09:25 bert4keras3-1.2.9.dist-info/RECORD
-12 files, 283508 bytes uncompressed, 58097 bytes compressed:  79.5%
+Zip file size: 43948 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      148 b- defN 24-Apr-25 09:18 bert4keras3/__init__.py
+-rw-rw-rw-  2.0 fat    23204 b- defN 24-Apr-25 09:17 bert4keras3/backend.py
+-rw-rw-rw-  2.0 fat    11442 b- defN 24-Apr-25 09:17 bert4keras3/layers.py
+-rw-rw-rw-  2.0 fat     5211 b- defN 24-Apr-25 09:17 bert4keras3/models.py
+-rw-rw-rw-  2.0 fat    30152 b- defN 24-Apr-25 09:17 bert4keras3/ops.py
+-rw-rw-rw-  2.0 fat    27955 b- defN 24-Apr-25 09:17 bert4keras3/snippets.py
+-rw-rw-rw-  2.0 fat    15509 b- defN 24-Apr-25 09:17 bert4keras3/tokenizers.py
+-rw-rw-rw-  2.0 fat    28534 b- defN 24-Apr-25 09:17 bert4keras3/transformers.py
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      219 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1037 b- defN 24-Apr-25 09:24 bert4keras3-1.3.dist-info/RECORD
+13 files, 154873 bytes uncompressed, 42240 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -15,23 +15,26 @@
 
 Filename: bert4keras3/snippets.py
 Comment: 
 
 Filename: bert4keras3/tokenizers.py
 Comment: 
 
-Filename: bert4keras3-1.2.9.dist-info/LICENSE
+Filename: bert4keras3/transformers.py
 Comment: 
 
-Filename: bert4keras3-1.2.9.dist-info/METADATA
+Filename: bert4keras3-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: bert4keras3-1.2.9.dist-info/WHEEL
+Filename: bert4keras3-1.3.dist-info/METADATA
 Comment: 
 
-Filename: bert4keras3-1.2.9.dist-info/top_level.txt
+Filename: bert4keras3-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: bert4keras3-1.2.9.dist-info/RECORD
+Filename: bert4keras3-1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: bert4keras3-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bert4keras3/__init__.py

```diff
@@ -1,6 +1,6 @@
 #! -*- coding: utf-8 -*-
 
-__version__ = '1.1.2'
+__version__ = '1.3'
 
 from bert4keras3 import backend,layers,models,snippets,tokenizers
 from bert4keras3.backend import ops
```

## bert4keras3/backend.py

```diff
@@ -80,14 +80,33 @@
     return ops.where(ops.isnan(y),ops.zeros_like(y),y)
 def int_shape(x):
     return ops.convert_to_numpy(x.shape)
 def gelu_erf(x):
     """基于Erf直接计算的gelu函数
     """
     return 0.5 * x * (1.0 + ops.erf(x / np.sqrt(2.0)))
+
+
+
+def integerize_shape(func):
+    """装饰器，保证input_shape一定是int或None
+    """
+    def convert(item):
+        if hasattr(item, '__iter__'):
+            return [convert(i) for i in item]
+        elif hasattr(item, 'value'):
+            return item.value
+        else:
+            return item
+
+    def new_func(self, input_shape):
+        input_shape = convert(input_shape)
+        return func(self, input_shape)
+
+    return new_func
 def set_gelu(version):
     """设置gelu版本
     """
     version = version.lower()
     assert version in ['erf', 'tanh'], 'gelu version must be erf or tanh'
     if version == 'erf':
         keras.utils.get_custom_objects()['gelu'] = gelu_erf
@@ -100,15 +119,15 @@
     t ∈ [1000, 2000]时，输出从1均匀降低到0.1，最后
     t > 2000时，保持0.1不变。
     """
     schedule = sorted(schedule.items())
     if from_zero and schedule[0][0] != 0:
         schedule = [(0, 0.0)] + schedule
 
-    t = ops.cast(t, K.floatx())
+    t = ops.cast(t, keras.mixed_precision.dtype_policy().name)
     x = (t * 0 + 1) * schedule[0][1]
     for i in range(len(schedule)):
         t_begin = schedule[i][0]
         x_begin = x
         if i != len(schedule) - 1:
             dx = schedule[i + 1][1] - schedule[i][1]
             dt = schedule[i + 1][0] - schedule[i][0]
@@ -202,16 +221,16 @@
     def where(cond, x, y):
         """给tf.where加上自动广播
         """
         shape = tf.broadcast_dynamic_shape(K.shape(x), K.shape(y))
         shape = tf.broadcast_dynamic_shape(K.shape(cond), shape)
     
         if dtype(x) is None and dtype(y) is None:
-            x = tf.broadcast_to(K.constant(x, dtype=K.floatx()), shape)
-            y = tf.broadcast_to(K.constant(y, dtype=K.floatx()), shape)
+            x = tf.broadcast_to(K.constant(x, dtype=keras.mixed_precision.dtype_policy().name), shape)
+            y = tf.broadcast_to(K.constant(y, dtype=keras.mixed_precision.dtype_policy().name), shape)
         elif dtype(x) is None:
             x = tf.broadcast_to(K.constant(x, dtype=dtype(y)), shape)
         elif dtype(y) is None:
             y = tf.broadcast_to(K.constant(y, dtype=dtype(x)), shape)
         else:
             x = tf.broadcast_to(x, shape)
             y = tf.broadcast_to(y, shape)
@@ -219,15 +238,46 @@
         if dtype(cond) != 'bool':
             cond = K.cast(cond, 'bool')
     
         cond = tf.broadcast_to(cond, shape)
         return tf.where(cond, x, y)
     ops.where = where
 
+def get_sequence_masking(
+    x, mask=None, value=0, axis=None, bias=None
+):
+    if not (mask is None and bias is None):
+        if mask is None:
+            if K.dtype(bias) == 'bool' or (backlib=='torch' and K.dtype(bias) == torch.bool):
+                mask = bias
+        else:
+            if axis is None:
+                axes = [1]
+            elif isinstance(axis, list):
+                axes = axis
+            else:
+                axes = [axis]
+
+            axes = [axis if axis >= 0 else ops.ndim(x) + axis for axis in axes]
 
+            if K.dtype(mask) != 'bool':
+                mask = ops.cast(mask, 'bool')
+            elif backlib=='torch' and K.dtype(bias) == torch.bool:
+                mask = ops.cast(mask, torch.bool)
+
+            full_mask = align(mask, [0, axes[0]], ops.ndim(x))
+            for axis in axes[1:]:
+                full_mask = full_mask & align(mask, [0, axis], ops.ndim(x))
+
+            mask = full_mask
+            if K.dtype(bias) == 'bool' or (backlib=='torch' and K.dtype(bias) == torch.bool):
+                mask = mask & bias
+    if mask is not None:
+        mask = ops.cast(mask,dtype='int32')
+    return mask
 def sequence_masking(
     x, mask=None, value=0, axis=None, bias=None, return_mask=False
 ):
     """为序列条件mask的函数
     mask: 形如(batch_size, seq_len)的bool矩阵；
     value: mask部分要被替换成的值，可以是'-inf'或'inf'；
     axis: 序列所在轴，默认为1；
@@ -305,67 +355,82 @@
 
 def attention_normalize(a, mask=None, axis=-1, method='softmax', bias=None):
     """不同的注意力归一化方案
     softmax：常规/标准的指数归一化；
     squared_relu：来自 https://arxiv.org/abs/2202.10447 ；
     softmax_plus：来自 https://kexue.fm/archives/8823 。
     """
+    if method == 'softmax-fp32' :
+        mask = get_sequence_masking(a, mask, -np.inf, axis,bias)
+        ori_dtype = a.dtype
+        att_mask = mask
+        for i in range(ops.ndim(a)-ops.ndim(mask)):
+            att_mask = ops.expand_dims(att_mask,0)
+        return ops.cast(keras.layers.Softmax(dtype="float32",axis=axis)(a,mask=att_mask),ori_dtype)
     a, mask = sequence_masking(a, mask, -np.inf, axis, bias, True)
+    
     if method == 'softmax' :
-        return ops.softmax(a, axis=axis)
+        return ops.softmax(a,axis=axis)
     else:
         if mask is None:
-            l = ops.cast(ops.shape(a)[-1], K.floatx())
+            l = ops.cast(ops.shape(a)[-1], keras.mixed_precision.dtype_policy().name)
         else:
-            mask = ops.cast(mask, K.floatx())
+            mask = ops.cast(mask, keras.mixed_precision.dtype_policy().name)
             l = ops.sum(mask, axis=axis, keepdims=True)
         if method == 'squared_relu':
             return ops.relu(a)**2 / l
         elif method == 'softmax_plus':
             l = ops.maximum(l, 16)  # 极短序列scale反而不好
             return ops.softmax(a * ops.log(l) / np.log(512), axis=axis)
     return a
 
 
 def sinusoidal_embeddings(pos, dim, base=10000):
     """计算pos位置的dim维sinusoidal编码
     """
     assert dim % 2 == 0
-    indices = ops.arange(0, dim // 2, dtype=K.floatx())
-    indices = ops.power(ops.cast(base, K.floatx()), -2 * indices / dim)
+    indices = ops.arange(0, dim // 2, dtype=keras.mixed_precision.dtype_policy().name)
+    indices = ops.power(ops.cast(base, keras.mixed_precision.dtype_policy().name), -2 * indices / dim)
     embeddings = ops.einsum('...,d->...d', pos, indices)
     embeddings = ops.stack([ops.sin(embeddings), ops.cos(embeddings)], axis=-1)
     embeddings = ops.flatten(embeddings, -2)
     return embeddings
 
 
 class Sinusoidal(keras.initializers.Initializer):
     """Sin-Cos位置向量初始化器
     来自：https://arxiv.org/abs/1706.03762
     """
     def __call__(self, shape, dtype=None):
         """Sin-Cos形式的位置向量
         """
         size, dim = shape
-        return sinusoidal_embeddings(ops.arange(size, dtype=K.floatx()), dim)
+        return sinusoidal_embeddings(ops.arange(size, dtype=keras.mixed_precision.dtype_policy().name), dim)
 def align(tensor, axes, ndim=None):
     """重新对齐tensor（批量版expand_dims）
     axes：原来的第i维对齐新tensor的第axes[i]维；
     ndim：新tensor的维度。
     """
     assert len(axes) == ops.ndim(tensor)
     assert ndim or min(axes) >= 0
     ndim = ndim or max(axes) + 1
     indices = [None] * ndim
     for i in axes:
         indices[i] = slice(None)
     if keras.__version__>'3.0' and os.environ["KERAS_BACKEND"] != "jax":
         return tensor[indices]
     return tensor[tuple(indices)]
-
+def _apply_rotary_pos_emb( tensor, cos_emb, sin_emb):
+        
+    x1, x2 = ops.split(tensor, 2, axis=-1)
+    half_rot_tensor = ops.stack((-x2, x1), axis=-2)
+    
+    half_rot_tensor = ops.reshape(half_rot_tensor, ops.shape(tensor))
+    
+    return (tensor * cos_emb) + (half_rot_tensor * sin_emb)
 
 def apply_rotary_position_embeddings(sinusoidal, *tensors):
     """应用RoPE到tensors中
     其中，sinusoidal.shape=[b, n, d]，tensors为tensor的列表，而
     tensor.shape=[b, n, ..., d]。
     """
     assert len(tensors) > 0, 'at least one input tensor'
@@ -378,16 +443,28 @@
     sin_pos = ops.repeat(sinusoidal[..., ::2], 2, -1)
     outputs = []
     for tensor in tensors:
         tensor2 = ops.stack([-tensor[..., 1::2], tensor[..., ::2]], ndim)
         tensor2 = ops.reshape(tensor2, ops.shape(tensor))
         outputs.append(tensor * cos_pos + tensor2 * sin_pos)
     return outputs[0] if len(outputs) == 1 else outputs
-
-
+def apply_rotary_position_embeddings_keras(sinusoidal, inputs):
+    ndim = ops.ndim(inputs)
+    sinusoidal = align(sinusoidal, [0, 1, -1], ndim)
+    dims = sinusoidal.shape[-1]
+    cos_emb = sinusoidal[..., :dims//2]
+    sin_emb = sinusoidal[..., dims//2:]
+    inputs = ops.moveaxis(
+            inputs, (-1, 1), (-1, 1)
+        )
+    
+    output = _apply_rotary_pos_emb(inputs, cos_emb, sin_emb)
+    return ops.moveaxis(
+            output, (-1, 1), (-1, 1)
+        )
 def multilabel_categorical_crossentropy(y_true, y_pred):
     """多标签分类的交叉熵
     说明：
         1. y_true和y_pred的shape一致，y_true的元素是0～1
            的数，表示当前类是目标类的概率；
         2. 请保证y_pred的值域是全体实数，换言之一般情况下
            y_pred不用加激活函数，尤其是不能加sigmoid或者
```

## bert4keras3/layers.py

```diff
@@ -1,61 +1,27 @@
 #! -*- coding: utf-8 -*-
 # 自定义层
 
 import numpy as np
 
-from bert4keras3.backend import keras, ops, is_tf_keras,K,tf,enable_flashatt
-if enable_flashatt:
-    from bert4keras3.backend import flash_mha
+from bert4keras3.backend import keras, ops, is_tf_keras,K,tf
 from bert4keras3.backend import align, sequence_masking,backlib
-from bert4keras3.backend import recompute_grad,int_shape
-from bert4keras3.backend import attention_normalize,divide_no_nan
-from bert4keras3.backend import sinusoidal_embeddings,slices_index
-from bert4keras3.backend import apply_rotary_position_embeddings
+from bert4keras3.backend import recompute_grad,int_shape,integerize_shape
 from keras import initializers, activations
 from keras.layers import *
 if keras.__version__<'3.0':
     from tensorflow import random
 else:
     from keras import random
-class TakeLayer(Layer):
-    def __init__(self, axis=0, **kwargs):
-        super(TakeLayer, self).__init__(**kwargs)
-        self.axis = axis
-    def get_config(self):
-        config = {
-            'axis': self.axis,
-        }
-        base_config = super(TakeLayer, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-    def call(self,inputs, **kwargs):
-        index = kwargs.get('index') 
-        att = kwargs.get('att')
-        out = ops.expand_dims(ops.take(inputs,index,self.axis),self.axis)
-        return out
-    def compute_output_shape(self, input_shape):
-        input_shape = list(input_shape)
-        input_shape[self.axis]=1
-        return input_shape
-def integerize_shape(func):
-    """装饰器，保证input_shape一定是int或None
-    """
-    def convert(item):
-        if hasattr(item, '__iter__'):
-            return [convert(i) for i in item]
-        elif hasattr(item, 'value'):
-            return item.value
-        else:
-            return item
-
-    def new_func(self, input_shape):
-        input_shape = convert(input_shape)
-        return func(self, input_shape)
-
-    return new_func
+from bert4keras3.Layers_add.sampler import *
+from bert4keras3.Layers_add.Embeddings import *
+from bert4keras3.Layers_add.GP import *
+from bert4keras3.Layers_add.LayerNorms import *
+from bert4keras3.Layers_add.Attentions import *
+from bert4keras3.Layers_add.FFN import *
 
 
 if (not is_tf_keras) and keras.__version__ < '2.3':
     import tensorflow as tf
     class Layer(keras.layers.Layer):
         """重新定义Layer，赋予“层中层”功能
         （仅keras 2.3以下版本需要）
@@ -147,15 +113,15 @@
 
 class GlobalAveragePooling1D(keras.layers.GlobalAveragePooling1D):
     """重新定义GlobalAveragePooling1D，支持序列长度为None
     """
     def call(self, inputs, mask=None):
         axis = 1 if self.data_format == 'channels_last' else 2
         if mask is not None:
-            mask = ops.cast(mask, K.floatx())
+            mask = ops.cast(mask, keras.mixed_precision.dtype_policy().name)
             mask = mask[..., None] if axis == 1 else mask[:, None]
             return ops.sum(inputs * mask, axis=axis) / ops.sum(mask, axis=axis)
         else:
             return ops.mean(inputs, axis=axis)
 
 
 class GlobalMaxPooling1D(keras.layers.GlobalMaxPooling1D):
@@ -174,191 +140,14 @@
         return None
 
 
 # 直接覆盖原对象
 keras.layers.GlobalAveragePooling1D = GlobalAveragePooling1D
 keras.layers.GlobalMaxPooling1D = GlobalMaxPooling1D
 
-
-def Input(
-    shape=None,
-    batch_size=None,
-    dtype=None,
-    sparse=None,
-    batch_shape=None,
-    name=None,
-    tensor=None,
-):
-    if dtype==None:
-        dtype='float32'
-    return keras.Input(
-        shape=shape,
-        batch_size=batch_size,
-        dtype=dtype,
-        sparse=sparse,
-        batch_shape=batch_shape,
-        name=name,
-        tensor=tensor,
-    )
-        
-        
-class Embedding(keras.layers.Embedding):
-    #def __init__(self, **kwargs):
-    #    super(Embedding, self).__init__(dtype='float32',**kwargs)
-
-    
-    def compute_mask(self, inputs, mask=None):
-        """为了适配T5，保证第一个token不被mask
-        """
-        #print(inputs)
-        if ops.ndim(inputs) == 2:
-            mask = super(Embedding, self).compute_mask(inputs, mask)
-            if mask is not None:
-                mask1 = ops.ones_like(mask[:, :1], dtype='bool')
-                mask2 = mask[:, 1:]
-                return ops.concatenate([mask1, mask2], 1)
-        else:
-            return mask
-
-    def call(self, inputs, mode='embedding'):
-        """新增mode参数，可以为embedding或dense。如果为embedding，
-        则等价于普通Embedding层；如果为dense，则等价于无bias的Dense层。
-        """
-        if mode == 'embedding':
-            
-            return super(Embedding, self).call(inputs)
-        else:
-            kernel = ops.transpose(self.embeddings)
-            return ops.dot(inputs, kernel)
-
-    def compute_output_shape(self, input_shape):
-        """关于判据，本来是通过缓存call时的mode参数来判断的，但是后来发现
-        Keras在使用compute_output_shape的时候不一定配套调用了call函数，
-        所以缓存的mode可能是不准的，因此只能出此下策。
-        """
-        if len(input_shape) == 2:
-            return super(Embedding, self).compute_output_shape(input_shape)
-        else:
-            return input_shape[:2] + (int_shape(self.embeddings)[0],)
-
-
-class ScaleOffset(Layer):
-    """简单的仿射变换层（最后一维乘上gamma向量并加上beta向量）
-    说明：1、具体操作为最后一维乘上gamma向量并加上beta向量；
-         2、如果直接指定scale和offset，那么直接常数缩放和平移；
-         3、hidden_*系列参数仅为有条件输入时(conditional=True)使用，
-            用于通过外部条件控制beta和gamma。
-    """
-    def __init__(
-        self,
-        scale=True,
-        offset=True,
-        conditional=False,
-        hidden_units=None,
-        hidden_activation='linear',
-        hidden_initializer='glorot_uniform',
-        **kwargs
-    ):
-        super(ScaleOffset, self).__init__(**kwargs)
-        self.scale = scale
-        self.offset = offset
-        self.conditional = conditional
-        self.hidden_units = hidden_units
-        self.hidden_activation = activations.get(hidden_activation)
-        self.hidden_initializer = initializers.get(hidden_initializer)
-
-    @integerize_shape
-    def build(self, input_shape):
-        super(ScaleOffset, self).build(input_shape)
-        
-        if self.conditional:
-            input_shape = input_shape[0]
-
-        if self.offset is True:
-            self.beta = self.add_weight(
-                name='beta', shape=(input_shape[-1],), initializer='zeros'
-            )
-        if self.scale is True:
-            self.gamma = self.add_weight(
-                name='gamma', shape=(input_shape[-1],), initializer='ones'
-            )
-
-        if self.conditional:
-
-            if self.hidden_units is not None:
-                self.hidden_dense = Dense(
-                    units=self.hidden_units,
-                    activation=self.hidden_activation,
-                    use_bias=False,
-                    kernel_initializer=self.hidden_initializer
-                )
-
-            if self.offset is not False and self.offset is not None:
-                self.beta_dense = Dense(
-                    units=input_shape[-1],
-                    use_bias=False,
-                    kernel_initializer='zeros'
-                )
-            if self.scale is not False and self.scale is not None:
-                self.gamma_dense = Dense(
-                    units=input_shape[-1],
-                    use_bias=False,
-                    kernel_initializer='zeros'
-                )
-
-    def compute_mask(self, inputs, mask=None):
-        if self.conditional:
-            return mask if mask is None else mask[0]
-        else:
-            return mask
-
-    @recompute_grad
-    def call(self, inputs):
-        """如果带有条件，则默认以list为输入，第二个是条件
-        """
-        if self.conditional:
-            inputs, conds = inputs
-            if self.hidden_units is not None:
-                conds = self.hidden_dense(conds)
-            conds = align(conds, [0, -1], ops.ndim(inputs))
-
-        if self.scale is not False and self.scale is not None:
-            gamma = self.gamma if self.scale is True else self.scale
-            if self.conditional:
-                gamma = gamma + self.gamma_dense(conds)
-            inputs = inputs * gamma
-
-        if self.offset is not False and self.offset is not None:
-            beta = self.beta if self.offset is True else self.offset
-            if self.conditional:
-                beta = beta + self.beta_dense(conds)
-            inputs = inputs + beta
-
-        return inputs
-
-    def compute_output_shape(self, input_shape):
-        if self.conditional:
-            return input_shape[0]
-        else:
-            return input_shape
-
-    def get_config(self):
-        config = {
-            'scale': self.scale,
-            'offset': self.offset,
-            'conditional': self.conditional,
-            'hidden_units': self.hidden_units,
-            'hidden_activation': activations.serialize(self.hidden_activation),
-            'hidden_initializer':
-                initializers.serialize(self.hidden_initializer),
-        }
-        base_config = super(ScaleOffset, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
 class Concatenate1D(Layer):
     """1维序列拼接层
     说明：本来该功能可以直接通过Concatenate层来实现，无奈Keras
          自带的Concatenate层的compute_mask写得不合理，导致一个
          带mask的序列与一个不带mask的序列拼接会报错，因此干脆
          自己重写一个好了。
     """
@@ -444,984 +233,29 @@
     def get_config(self):
         config = {
             'parts': self.parts,
         }
         base_config = super(BatchSplit, self).get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
-
 class BatchConcat(Layer):
     """将第一维进行合并
     主要是用于自行实现多卡数据并行。
     """
     def compute_mask(self, inputs, mask=None):
         if isinstance(mask, list):
             if all([m is not None for m in mask]):
                 return ops.concatenate(mask, 0)
 
     def call(self, inputs):
         return ops.concatenate(inputs, 0)
 
     def compute_output_shape(self, input_shape):
         return input_shape[0]
-class SearchBase(Layer):
-    def __init__(self, end_token,k=1, **kwargs):
-        super(SearchBase, self).__init__(**kwargs)
-        self.k = k
-        self.end_token=end_token
-    def get_config(self):
-        config = {
-            'k': self.k,
-            'end_token':self.end_token
-        }
-        base_config = super(SearchBase, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-    def sample(self,x):
-        x = ops.cast(ops.log(x), "float32")
-        
-        return keras.random.categorical(
-            # tf does not support half precision multinomial sampling, so make
-            # sure we have full precision here.
-            x,
-            1,
-            seed=np.random.randint(1,2147483648),
-            dtype="int32",
-        )
-        
-class GreedySearch(SearchBase):
-    def search(self,t):
-        return ops.argmax(t,-1)
-    def call(self, inputs, **kwargs):
-        hidden_state,update_index,out_ids,flags = inputs[:]
-        
-        y = self.search(hidden_state)
-        t = ops.full_like(y,self.end_token)
-        y = ops.where(flags,y,t)
-        start = [0,update_index]
-        flags = y!=self.end_token
-
-        return ops.slice_update(out_ids,start,ops.cast(y,out_ids.dtype)),flags
-    
-class TopkSearch(GreedySearch):
-    def search(self,t):
-        top_k_pred, top_k_indices = ops.top_k(
-            t[:,0],
-            k=self.k,
-            sorted=False,
-        )
-        
-        sample_indices = self.sample(top_k_pred)
-
-        return ops.take_along_axis(top_k_indices, sample_indices, axis=-1)
-
-class ToppSearch(TopkSearch):
-    def search(self,t):
-        cutoff = ops.shape(t)[-1]
-        sorted_preds, sorted_indices = ops.top_k(
-            t[:,0], k=cutoff, sorted=True
-        )
-        # Calculate cumulative probability distribution.
-        cumulative_probabilities = ops.cumsum(sorted_preds, axis=-1)
-        # Create a mask for the tokens to keep.
-        keep_mask = cumulative_probabilities <= self.k
-        # Shift to include the last token that exceed p.
-        shifted_keep_mask = ops.concatenate(
-            [ops.ones_like(keep_mask[:, :1]), keep_mask[:, :-1]], axis=1
-        )
-        # Filter out unmasked tokens and sample from filtered distribution.
-        probabilities = ops.where(
-            shifted_keep_mask,
-            sorted_preds,
-            ops.zeros(ops.shape(sorted_preds), dtype=sorted_preds.dtype),
-        )
-        sorted_next_token = self.sample(probabilities)
-        output = ops.take_along_axis(sorted_indices, sorted_next_token, axis=-1)
-        return output
-class MultiHeadAttention(Layer):
-    """多头注意力机制
-    """
-    def __init__(
-        self,
-        heads,
-        head_size,
-        out_dim=None,
-        key_size=None,
-        use_bias=True,
-        normalization='softmax',
-        attention_scale=True,
-        attention_dropout=None,
-        return_attention_scores=False,
-        kernel_initializer='glorot_uniform',
-        **kwargs
-    ):
-        super(MultiHeadAttention, self).__init__(**kwargs)
-        self.heads = heads
-        self.head_size = head_size
-        self.out_dim = out_dim or heads * head_size
-        self.key_size = key_size or head_size
-        self.use_bias = use_bias
-        self.normalization = normalization
-        self.attention_scale = attention_scale
-        self.attention_dropout = attention_dropout
-        self.return_attention_scores = return_attention_scores
-        self.kernel_initializer = initializers.get(kernel_initializer)
-
-    def build(self, input_shape):
-        
-        self.q_dense = Dense(
-            units=self.key_size * self.heads,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-            
-        )
-        self.k_dense = Dense(
-            units=self.key_size * self.heads,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-        self.v_dense = Dense(
-            units=self.head_size * self.heads,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-        self.o_dense = Dense(
-            units=self.out_dim,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-        if self.attention_dropout:
-            self.dropout=Dropout(self.attention_dropout)
-        super(MultiHeadAttention, self).build(input_shape)
-    @recompute_grad
-    def call(self, inputs, mask=None, **kwargs):
-        """实现多头注意力
-        q_mask: 对输入的query序列的mask。
-                主要是将输出结果的padding部分置0。
-        v_mask: 对输入的value序列的mask。
-                主要是防止attention读取到padding信息。
-        """
-        q, k, v = inputs[:3]
-        q_mask, v_mask = None, None
-        use_cache = kwargs.get('use_cache')
-        if mask is not None:
-            q_mask, v_mask = mask[0], mask[2]
-        # 线性变换
-        qw = self.q_dense(q)
-        kw = self.k_dense(k)
-        vw = self.v_dense(v)
-        # 形状变换
-        qw = ops.reshape(qw, (self.heads, self.key_size), -1)
-        kw = ops.reshape(kw, (self.heads, self.key_size), -1)
-        vw = ops.reshape(vw, (self.heads, self.head_size), -1)
-        # Attention
-        qkv_inputs = [qw, kw, vw] + inputs[3:]
-        qv_masks = [q_mask, v_mask]
-        
-        o, a,cache = self.pay_attention_to(qkv_inputs, qv_masks, **kwargs)
-        # 完成输出
-        o = self.o_dense(ops.flatten(o, 2))
-        # 返回结果
-         
-        
-        if use_cache:
-            return o,cache
-        if self.return_attention_scores:
-            return [o, a]
-        else:
-            return o
-
-    def pay_attention_to(self, inputs, mask=None, **kwargs):
-        """实现标准的乘性多头注意力
-        a_bias: 对attention矩阵的bias。
-                不同的attention bias对应不同的应用。
-        p_bias: 在attention里的位置偏置。
-                一般用来指定相对位置编码的种类。
-        说明: 这里单独分离出pay_attention_to函数，是为了方便
-              继承此类来定义不同形式的attention；此处要求
-              返回o.shape=(batch_size, seq_len, heads, head_size)。
-        """
-        (qw, kw, vw), n = inputs[:3], 3
-        
-        q_mask, v_mask = mask
-        a_bias, p_bias = kwargs.get('a_bias'), kwargs.get('p_bias')
-        is_cache_update_index = kwargs.get('cache_update_index')
-        use_cache = kwargs.get('use_cache')
-        if a_bias:
-            a_bias = inputs[n]
-            n += 1
-        
-        if p_bias == 'rotary':
-            
-            #print(inputs[n].shape, qw.shape, kw.shape)
-            qw, kw = apply_rotary_position_embeddings(inputs[n], qw, kw)
-            n += 1
-        if use_cache:
-            cache = inputs[n]
-            n +=1
-            key_cache = cache[:, 0, ...]
-            value_cache = cache[:, 1, ...]
-            if is_cache_update_index:
-                cache_update_index = inputs[n]
-                n += 1
-                start = [0, cache_update_index, 0, 0]
-                #print(key_cache.shape, start, kw.shape)
-                kw = ops.slice_update(key_cache, start, kw)
-                vw = ops.slice_update(value_cache, start, vw)
-                cache = ops.stack((kw, vw), axis=1)
-            else:
-                kw = key_cache
-                vw = value_cache
-        else:
-            cache = None
-        
-        if enable_flashatt:
-            is_causal = False
-            if a_bias is not None:
-                is_causal = True
-            softmax_scale = 1.
-            if self.attention_scale:
-                softmax_scale = 1 / self.key_size**0.5
-            o = flash_mha(qw,kw,vw,softmax_scale=softmax_scale, is_causal=is_causal)
-            return o,[],[]
-        # Attention
-        a = ops.einsum('bjhd,bkhd->bhjk', qw, kw)
-        # 处理位置编码
-        if p_bias == 'typical_relative':
-            position_bias = inputs[n]
-            a = a + ops.einsum('bjhd,jkd->bhjk', qw, position_bias)
-        elif p_bias == 't5_relative':
-            position_bias = ops.transpose(inputs[n], (2, 0, 1))
-            #print(a.shape,position_bias.shape)
-            a = a + ops.expand_dims(position_bias, 0)
-        # Attention（续）
-        if self.attention_scale:
-            a = a / self.key_size**0.5
-        if a_bias is not None and ops.ndim(a_bias) == 3:
-            a_bias = align(a_bias, [0, -2, -1], ops.ndim(a))
-        A = attention_normalize(a, v_mask, -1, self.normalization, a_bias)
-        
-        if self.attention_dropout:
-            A = self.dropout(A)
-        # 完成输出
-
-        o = ops.einsum('bhjk,bkhd->bjhd', A, vw)
-        if p_bias == 'typical_relative':
-            o = o + ops.einsum('bhjk,jkd->bjhd', A, position_bias)
-        
-        return o,a,cache
-
-    
-    def compute_output_shape(self, input_shape):
-        o_shape = (input_shape[0][0], input_shape[0][1], self.out_dim)
-        for shape in input_shape:
-            if len(shape)==5 and shape[1]==2:
-                return [o_shape,shape]
-        if self.return_attention_scores:
-            a_shape = (
-                input_shape[0][0], self.heads, input_shape[0][1],
-                input_shape[1][1]
-            )
-            return [o_shape, a_shape]
-        else:
-            return o_shape
-    
-    def compute_mask(self, inputs, mask=None):
-        if mask is not None:
-            if self.return_attention_scores:
-                return [mask[0], None]
-            else:
-                return mask[0]
-
-    def get_config(self):
-        config = {
-            'heads': self.heads,
-            'head_size': self.head_size,
-            'out_dim': self.out_dim,
-            'key_size': self.key_size,
-            'use_bias': self.use_bias,
-            'normalization': self.normalization,
-            'attention_scale': self.attention_scale,
-            'attention_dropout': self.attention_dropout,
-            'return_attention_scores': self.return_attention_scores,
-            'kernel_initializer':
-                initializers.serialize(self.kernel_initializer),
-        }
-        base_config = super(MultiHeadAttention, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class GatedAttentionUnit(Layer):
-    """门控注意力单元
-    链接：https://arxiv.org/abs/2202.10447
-    介绍：https://kexue.fm/archives/8934
-    说明：没有加入加性相对位置编码，个人认为是不必要的；如果觉得有必要，
-         可以自行通过a_bias传入。
-    """
-    def __init__(
-        self,
-        units,
-        key_size,
-        activation='swish',
-        use_bias=True,
-        normalization='squared_relu',
-        self_attention=True,
-        attention_scale=True,
-        attention_dropout=None,
-        kernel_initializer='glorot_uniform',
-        factorization=False,#是否把V做分解
-        **kwargs
-    ):
-        super(GatedAttentionUnit, self).__init__(**kwargs)
-        self.units = units
-        self.key_size = key_size
-        self.activation = activations.get(activation)
-        self.use_bias = use_bias
-        self.normalization = normalization
-        self.self_attention = self_attention
-        self.attention_scale = attention_scale
-        self.attention_dropout = attention_dropout
-        self.kernel_initializer = initializers.get(kernel_initializer)
-        self.factorization = factorization
-    @integerize_shape
-    def build(self, input_shape):
-        super(GatedAttentionUnit, self).build(input_shape)
-        hidden_size = input_shape[-1]
-        if isinstance(hidden_size, (list, tuple)):
-            hidden_size = input_shape[0][-1]
-        if self.self_attention:
-            self.i_dense = Dense(
-                units=2 * self.units + self.key_size,
-                activation=self.activation,
-                use_bias=self.use_bias,
-                kernel_initializer=self.kernel_initializer
-            )
-            self.q_scaleoffset = ScaleOffset(offset=self.use_bias)
-            self.k_scaleoffset = ScaleOffset(offset=self.use_bias)
-        else:
-            
-            self.u_dense = Dense(
-                units=self.units ,
-                activation=self.activation,
-                use_bias=self.use_bias,
-                kernel_initializer=self.kernel_initializer
-            )
-            self.q_dense = Dense(
-                units=self.key_size,
-                activation=self.activation,
-                use_bias=self.use_bias,
-                kernel_initializer=self.kernel_initializer
-            )
-            self.k_dense = Dense(
-                units=self.key_size,
-                activation=self.activation,
-                use_bias=self.use_bias,
-                kernel_initializer=self.kernel_initializer
-            )
-            if self.factorization:
-                self.v_dense = Dense(
-                    units=self.key_size,
-                    activation='linear',
-                    use_bias=False,
-                    kernel_initializer=self.kernel_initializer
-                )
-                self.vW_dense = Dense(
-                    units=self.units,
-                    activation='linear',
-                    use_bias=False,
-                    kernel_initializer=self.kernel_initializer
-                )
-            else:
-                self.v_dense = Dense(
-                    units=self.units,
-                    activation=self.activation,
-                    use_bias=self.use_bias,
-                    kernel_initializer=self.kernel_initializer
-                )
-        self.o_dense = Dense(
-            units=hidden_size,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-            
-        if self.attention_dropout:
-            self.dropout=Dropout(self.attention_dropout)
-    @recompute_grad
-    def call(self, inputs, mask=None, a_bias=None, p_bias=None):
-        
-        if not isinstance(inputs, list):
-            inputs, mask = [inputs], [mask]
-        if self.self_attention:
-            x, n = inputs[0], 1
-        else:
-            
-            (q, k, v), n = inputs[:3], 3
-        mask = None if mask is None else mask[0]
-        if a_bias:
-            a_bias = inputs[n]
-            n += 1
-        # 投影变换
-        if self.self_attention:
-            x = self.i_dense(x)
-            u, v, qk = x[:,:,:self.units],x[:,:,self.units:self.units*2],x[:,:,self.units*2:]
-            q, k = self.q_scaleoffset(qk), self.k_scaleoffset(qk)
-        else:
-            u, q = self.u_dense(q),self.q_dense(q)
-            k, v = self.k_dense(k), self.v_dense(v)
-        # 加入RoPE
-        if p_bias == 'rotary':
-            q, k = apply_rotary_position_embeddings(inputs[n], q, k)
-        # Attention
-        if enable_flashatt and ops.shape(k)==ops.shape(v):
-            z = self.pay_flash_attention_to(q,k,v, a_bias)
-        else:
-            z = self.pay_attention_to(q,k,v,mask, a_bias)   
-        # 计算输出
-        if self.self_attention==False and self.factorization:
-            z = self.vW_dense(z)
-        o = self.o_dense(u * z)
-        return o
-    def pay_flash_attention_to(self, q,k,v, a_bias):
-        is_causal = False
-        if a_bias is not None:
-            is_causal = True
-        softmax_scale = 1.
-        if self.attention_scale:
-            softmax_scale = 1 / self.key_size**0.5
-        if ops.ndim(q)==3:
-            k = ops.expand_dims(k,2)
-            q = ops.expand_dims(q,2)
-            v = ops.expand_dims(v,2)
-        o = flash_mha(q,k,v,softmax_scale=softmax_scale, is_causal=is_causal)
-        return ops.squeeze(o,2)
-    def pay_attention_to(self, q,k,v,mask, a_bias):
-        a = ops.einsum('bmd,bnd->bmn', q, k)
-        if self.attention_scale:
-            a = a / self.key_size**0.5
-        A = attention_normalize(a, mask, -1, self.normalization, a_bias)
-        if self.attention_dropout:
-            A = self.dropout(A)
-        try:
-            z=ops.einsum('bmn,bnd->bmd', A, v)
-        except:
-            pass
-        return z
-
-    def compute_mask(self, inputs, mask=None):
-        if isinstance(mask, list):
-            return mask[0]
-        else:
-            return mask
-
-    def compute_output_shape(self, input_shape):
-        if isinstance(input_shape[0], (list, tuple)):
-            return input_shape[0]
-        else:
-            return input_shape
-
-    def get_config(self):
-        config = {
-            'units': self.units,
-            'key_size': self.key_size,
-            'activation': activations.serialize(self.activation),
-            'use_bias': self.use_bias,
-            'normalization': self.normalization,
-            'self_attention': self.self_attention,
-            'attention_scale': self.attention_scale,
-            'attention_dropout': self.attention_dropout,
-            'kernel_initializer':
-                initializers.serialize(self.kernel_initializer),
-        }
-        base_config = super(GatedAttentionUnit, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class LayerNormalization(ScaleOffset):
-    """(Conditional) Layer Normalization
-    """
-    def __init__(
-        self, zero_mean=True, unit_variance=True, epsilon=None, **kwargs
-    ):
-        super(LayerNormalization, self).__init__(**kwargs)
-        self.zero_mean = zero_mean
-        self.unit_variance = unit_variance
-        self.epsilon = epsilon or K.epsilon()
-
-    @recompute_grad
-    def call(self, inputs):
-        """如果是条件Layer Norm，则默认以list为输入，第二个是条件
-        """
-        
-        if self.conditional:
-            inputs, conds = inputs
-
-        if self.zero_mean:
-            mean = ops.mean(inputs, axis=-1, keepdims=True)
-            inputs = inputs - mean
-            
-        if self.unit_variance:
-            variance = ops.mean(ops.square(inputs), axis=-1, keepdims=True)
-            
-            inputs = divide_no_nan(
-                inputs, ops.sqrt(variance + self.epsilon)
-            )
-        if self.conditional:
-            inputs = [inputs, conds]
-
-        return super(LayerNormalization, self).call(inputs)
-
-    def get_config(self):
-        config = {
-            'zero_mean': self.zero_mean,
-            'unit_variance': self.unit_variance,
-            'epsilon': self.epsilon,
-        }
-        base_config = super(LayerNormalization, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class PositionEmbedding(Layer):
-    """定义可训练的位置Embedding
-    """
-    def __init__(
-        self,
-        input_dim,
-        output_dim,
-        merge_mode='add',
-        hierarchical=None,
-        embeddings_initializer='zeros',
-        custom_position_ids=False,
-        **kwargs
-    ):
-        super(PositionEmbedding, self).__init__(**kwargs)
-        self.input_dim = input_dim
-        self.output_dim = output_dim
-        self.merge_mode = merge_mode
-        self.hierarchical = hierarchical
-        self.embeddings_initializer = initializers.get(embeddings_initializer)
-        self.custom_position_ids = custom_position_ids
-
-    def build(self, input_shape):
-        super(PositionEmbedding, self).build(input_shape)
-        self.embeddings = self.add_weight(
-            name='embeddings',
-            shape=(self.input_dim, self.output_dim),
-            initializer=self.embeddings_initializer
-        )
-
-    def call(self, inputs):
-        """如果custom_position_ids，那么第二个输入为自定义的位置id
-        """
-        flag = isinstance(inputs,list)
-        if self.custom_position_ids or flag :
-            inputs, position_ids = inputs
-            position_ids = ops.cast(position_ids, 'int32')
-        else:
-            input_shape = ops.shape(inputs)
-            batch_size, seq_len = input_shape[0], input_shape[1]
-            position_ids = ops.arange(0, seq_len, dtype='int32')[None]
-
-        if self.hierarchical:
-            alpha = 0.4 if self.hierarchical is True else self.hierarchical
-            embeddings = self.embeddings - alpha * self.embeddings[:1]
-            embeddings = embeddings / (1 - alpha)
-            embeddings_x = ops.take(embeddings, position_ids // self.input_dim)
-            embeddings_y = ops.take(embeddings, position_ids % self.input_dim)
-            embeddings = alpha * embeddings_x + (1 - alpha) * embeddings_y
-        else:
-            if self.custom_position_ids or flag :
-                embeddings = ops.take(self.embeddings, position_ids,axis=0)
-            else:
-                embeddings = self.embeddings[None, :seq_len]
-
-        if self.merge_mode == 'add':
-            return inputs + embeddings
-        elif self.merge_mode == 'mul':
-            return inputs * (embeddings + 1.0)
-        elif self.merge_mode == 'zero':
-            return embeddings
-        else:
-            if not self.custom_position_ids:
-                embeddings = ops.tile(embeddings, [batch_size, 1, 1])
-            return ops.concatenate([inputs, embeddings])
-
-    def compute_output_shape(self, input_shape):
-        if self.custom_position_ids:
-            input_shape = input_shape[0]
-
-        if self.merge_mode in ['add', 'mul', 'zero']:
-            return input_shape[:2] + (self.output_dim,)
-        else:
-            return input_shape[:2] + (input_shape[2] + self.output_dim,)
-
-    def get_config(self):
-        config = {
-            'input_dim': self.input_dim,
-            'output_dim': self.output_dim,
-            'merge_mode': self.merge_mode,
-            'hierarchical': self.hierarchical,
-            'embeddings_initializer':
-                initializers.serialize(self.embeddings_initializer),
-            'custom_position_ids': self.custom_position_ids,
-        }
-        base_config = super(PositionEmbedding, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class SinusoidalPositionEmbedding(Layer):
-    """定义Sin-Cos位置Embedding
-    """
-    def __init__(
-        self,
-        output_dim,
-        merge_mode='add',
-        custom_position_ids=False,
-        **kwargs
-    ):
-        super(SinusoidalPositionEmbedding, self).__init__(**kwargs)
-        self.output_dim = output_dim
-        self.merge_mode = merge_mode
-        self.custom_position_ids = custom_position_ids
-
-    def call(self, inputs):
-        
-        """如果custom_position_ids，那么第二个输入为自定义的位置id
-        """
-        if self.custom_position_ids:
-            inputs, position_ids = inputs
-            if 'float' not in K.dtype(position_ids):
-                position_ids = ops.cast(position_ids, K.floatx())
-        else:
-            input_shape = ops.shape(inputs)
-            batch_size, seq_len = input_shape[0], input_shape[1]
-            position_ids = ops.arange(0, seq_len, dtype=K.floatx())[None]
-
-        embeddings = sinusoidal_embeddings(position_ids, self.output_dim)
-        
-        if self.merge_mode == 'add':
-            return inputs + embeddings
-        elif self.merge_mode == 'mul':
-            return inputs * (embeddings + 1.0)
-        elif self.merge_mode == 'zero':
-            return embeddings
-        else:
-            if not self.custom_position_ids:
-                embeddings = ops.tile(embeddings, [batch_size, 1, 1])
-            return ops.concatenate([inputs, embeddings])
-
-    def compute_output_shape(self, input_shape):
-        if self.custom_position_ids:
-            input_shape = input_shape[0]
-
-        if self.merge_mode in ['add', 'mul', 'zero']:
-            return input_shape[:2] + (self.output_dim,)
-        else:
-            return input_shape[:2] + (input_shape[2] + self.output_dim,)
-
-    def get_config(self):
-        config = {
-            'output_dim': self.output_dim,
-            'merge_mode': self.merge_mode,
-            'custom_position_ids': self.custom_position_ids,
-        }
-        base_config = super(SinusoidalPositionEmbedding, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class RelativePositionEmbedding(Layer):
-    """相对位置编码
-    来自论文：https://arxiv.org/abs/1803.02155
-    """
-    def __init__(
-        self, input_dim, output_dim, embeddings_initializer='zeros', **kwargs
-    ):
-        super(RelativePositionEmbedding, self).__init__(**kwargs)
-        self.input_dim = input_dim
-        self.output_dim = output_dim
-        self.embeddings_initializer = initializers.get(embeddings_initializer)
-
-    def build(self, input_shape):
-        super(RelativePositionEmbedding, self).build(input_shape)
-        self.embeddings = self.add_weight(
-            name='embeddings',
-            shape=(self.input_dim, self.output_dim),
-            initializer=self.embeddings_initializer,
-        )
-
-    def call(self, inputs):
-        pos_ids = self.compute_position_ids(inputs)
-        return ops.take(self.embeddings,ops.cast(pos_ids,'int32'),axis=0)
-
-    def compute_position_ids(self, inputs):
-        q, v = inputs
-        # 计算位置差
-        q_idxs = ops.arange(0, ops.shape(q)[1], dtype='int32')
-        q_idxs = ops.expand_dims(q_idxs, 1)
-        v_idxs = ops.arange(0, ops.shape(v)[1], dtype='int32')
-        v_idxs = ops.expand_dims(v_idxs, 0)
-        pos_ids = v_idxs - q_idxs
-        # 后处理操作
-        max_position = (self.input_dim - 1) // 2
-        pos_ids = ops.clip(pos_ids, -max_position, max_position)
-        pos_ids = pos_ids + max_position
-        return pos_ids
-
-    def compute_output_shape(self, input_shape):
-        return (input_shape[0][1], input_shape[1][1], self.output_dim)
-
-    def compute_mask(self, inputs, mask):
-        if mask!=None:
-            return mask[0]
-        return mask
-
-    def get_config(self):
-        config = {
-            'input_dim': self.input_dim,
-            'output_dim': self.output_dim,
-            'embeddings_initializer':
-                initializers.serialize(self.embeddings_initializer),
-        }
-        base_config = super(RelativePositionEmbedding, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
 
-class RelativePositionEmbeddingT5(RelativePositionEmbedding):
-    """Google T5的相对位置编码
-    来自论文：https://arxiv.org/abs/1910.10683
-    """
-    def __init__(
-        self,
-        input_dim,
-        output_dim,
-        max_distance=128,
-        bidirectional=True,
-        embeddings_initializer='zeros',
-        **kwargs
-    ):
-        super(RelativePositionEmbeddingT5,
-              self).__init__(input_dim, output_dim, **kwargs)
-        self.max_distance = max_distance
-        self.bidirectional = bidirectional
-
-    def compute_position_ids(self, inputs):
-        """T5的相对位置分桶（直接翻译自官方T5源码）
-        """
-        q, v = inputs
-        # 计算位置差
-        q_idxs = ops.arange(0, ops.shape(q)[1], dtype='int32')
-        q_idxs = ops.expand_dims(q_idxs, 1)
-        v_idxs = ops.arange(0, ops.shape(v)[1], dtype='int32')
-        v_idxs = ops.expand_dims(v_idxs, 0)
-        pos_ids = v_idxs - q_idxs
-        # 后处理操作
-        num_buckets, max_distance = self.input_dim, self.max_distance
-        ret = 0
-        n = -pos_ids
-        if self.bidirectional:
-            num_buckets //= 2
-            ret += ops.cast(ops.less(n, 0), 'int32') * num_buckets
-            n = ops.absolute(n)
-        else:
-            n = ops.maximum(n, 0)
-        # now n is in the range [0, inf)
-        max_exact = num_buckets // 2
-        is_small = ops.less(n, max_exact)
-        val_if_large = max_exact + ops.cast(
-            ops.log(ops.cast(n, K.floatx()) / max_exact) /
-            np.log(max_distance / max_exact) * (num_buckets - max_exact),
-            'int32',
-        )
-        val_if_large = ops.minimum(val_if_large, num_buckets - 1)
-        ret += ops.where(is_small, n, val_if_large)
-        return ret
-
-    def get_config(self):
-        config = {
-            'max_distance': self.max_distance,
-            'bidirectional': self.bidirectional,
-        }
-        base_config = super(RelativePositionEmbeddingT5, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class FeedForward(Layer):
-    """FeedForward层
-    如果activation不是一个list，那么它就是两个Dense层的叠加；如果activation是
-    一个list，那么第一个Dense层将会被替换成门控线性单元（Gated Linear Unit）。
-    参考论文: https://arxiv.org/abs/2002.05202
-    """
-    def __init__(
-        self,
-        units,
-        activation='relu',
-        use_bias=True,
-        kernel_initializer='glorot_uniform',
-        **kwargs
-    ):
-        super(FeedForward, self).__init__(**kwargs)
-        self.units = units
-        if not isinstance(activation, list):
-            activation = [activation]
-        self.activation = [activations.get(act) for act in activation]
-        self.use_bias = use_bias
-        self.kernel_initializer = initializers.get(kernel_initializer)
-
-    @integerize_shape
-    def build(self, input_shape):
-        super(FeedForward, self).build(input_shape)
-        output_dim = input_shape[-1]
-
-        for i, activation in enumerate(self.activation):
-            i_dense = Dense(
-                units=self.units,
-                activation=activation,
-                use_bias=self.use_bias,
-                kernel_initializer=self.kernel_initializer
-            )
-            setattr(self, 'i%s_dense' % i, i_dense)
-
-        self.o_dense = Dense(
-            units=output_dim,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-
-    @recompute_grad
-    def call(self, inputs):
-        x = self.i0_dense(inputs)
-        for i in range(1, len(self.activation)):
-            x = x * getattr(self, 'i%s_dense' % i)(inputs)
-        x = self.o_dense(x)
-        return x
-
-    def get_config(self):
-        config = {
-            'units': self.units,
-            'activation': [
-                activations.serialize(act) for act in self.activation
-            ],
-            'use_bias': self.use_bias,
-            'kernel_initializer':
-                initializers.serialize(self.kernel_initializer),
-        }
-        base_config = super(FeedForward, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-
-class GlobalPointer(Layer):
-    """全局指针模块
-    将序列的每个(start, end)作为整体来进行判断
-    参考：https://kexue.fm/archives/8373
-    """
-    def __init__(
-        self,
-        heads,
-        head_size,
-        RoPE=True,
-        use_bias=True,
-        tril_mask=True,
-        kernel_initializer='lecun_normal',
-        **kwargs
-    ):
-        super(GlobalPointer, self).__init__(**kwargs)
-        self.heads = heads
-        self.head_size = head_size
-        self.RoPE = RoPE
-        self.use_bias = use_bias
-        self.tril_mask = tril_mask
-        self.kernel_initializer = initializers.get(kernel_initializer)
-
-    def build(self, input_shape):
-        super(GlobalPointer, self).build(input_shape)
-        self.dense = Dense(
-            units=self.head_size * self.heads * 2,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-
-    def compute_mask(self, inputs, mask=None):
-        return None
-
-    @recompute_grad
-    def call(self, inputs, mask=None):
-        # 输入变换
-        inputs = self.dense(inputs)
-        inputs = ops.split(inputs, self.heads, axis=-1)
-        inputs = ops.stack(inputs, axis=-2)
-        qw, kw = inputs[..., :self.head_size], inputs[..., self.head_size:]
-        # RoPE编码
-        if self.RoPE:
-            pos = SinusoidalPositionEmbedding(self.head_size, 'zero')(inputs)
-            qw, kw = apply_rotary_position_embeddings(pos, qw, kw)
-        # 计算内积
-        logits = ops.einsum('bmhd,bnhd->bhmn', qw, kw) / self.head_size**0.5
-        # 排除下三角
-        if self.tril_mask:
-            tril_mask = ops.triu(ops.ones_like(logits[0, 0]))
-            tril_mask = ops.cast(tril_mask, 'bool')
-        else:
-            tril_mask = None
-        # 返回最终结果
-        return sequence_masking(logits, mask, -np.inf, [2, 3], tril_mask)
-
-    def compute_output_shape(self, input_shape):
-        return (input_shape[0], self.heads, input_shape[1], input_shape[1])
-
-    def get_config(self):
-        config = {
-            'heads': self.heads,
-            'head_size': self.head_size,
-            'RoPE': self.RoPE,
-            'use_bias': self.use_bias,
-            'tril_mask': self.tril_mask,
-            'kernel_initializer':
-                initializers.serialize(self.kernel_initializer),
-        }
-        base_config = super(GlobalPointer, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class EfficientGlobalPointer(GlobalPointer):
-    """更加参数高效的GlobalPointer
-    参考：https://kexue.fm/archives/8877
-    """
-    def build(self, input_shape):
-        self.p_dense = Dense(
-            units=self.head_size * 2,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-        self.q_dense = Dense(
-            units=self.heads * 2,
-            use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer
-        )
-        self.built = True
-
-    @recompute_grad
-    def call(self, inputs, mask=None):
-        # 输入变换
-        inputs = self.p_dense(inputs)
-        qw, kw = inputs[..., ::2], inputs[..., 1::2]
-        # RoPE编码
-        if self.RoPE:
-            pos = SinusoidalPositionEmbedding(self.head_size, 'zero')(inputs)
-            qw, kw = apply_rotary_position_embeddings(pos, qw, kw)
-        # 计算内积
-        logits = ops.einsum('bmd,bnd->bmn', qw, kw) / self.head_size**0.5
-        bias = ops.einsum('bnh->bhn', self.q_dense(inputs)) / 2
-        logits = logits[:, None] + bias[:, ::2, None] + bias[:, 1::2, :, None]
-        # 排除下三角
-        if self.tril_mask:
-            tril_mask = ops.triu(ops.ones_like(logits[0, 0]))
-            tril_mask = ops.cast(tril_mask, 'bool')
-        else:
-            tril_mask = None
-        # 返回最终结果
-        return sequence_masking(logits, mask, -np.inf, [2, 3], tril_mask)
 
 
 class Loss(Layer):
     """特殊的层，用来定义复杂loss
     """
     def __init__(self, output_axis=None, **kwargs):
         super(Loss, self).__init__(**kwargs)
@@ -1460,14 +294,35 @@
     def get_config(self):
         config = {
             'output_axis': self.output_axis,
         }
         base_config = super(Loss, self).get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
+def Input(
+    shape=None,
+    batch_size=None,
+    dtype=None,
+    sparse=None,
+    batch_shape=None,
+    name=None,
+    tensor=None,
+    ):
+    if dtype==None:
+        dtype='float32'
+    return keras.Input(
+            shape=shape,
+            batch_size=batch_size,
+            dtype=dtype,
+            sparse=sparse,
+            batch_shape=batch_shape,
+            name=name,
+            tensor=tensor,
+            )
+keras.layers.Input = Input
 
 custom_objects = {
     'Embedding': Embedding,
     'ScaleOffset': ScaleOffset,
     'Concatenate1D': Concatenate1D,
     'BatchSplit': BatchSplit,
     'BatchConcat': BatchConcat,
```

## bert4keras3/models.py

```diff
@@ -1,3253 +1,21 @@
 #! -*- coding: utf-8 -*-
 # 主要模型
 
-import numpy as np
-from bert4keras3.backend import tf,keras,backlib,lora_model
-from bert4keras3.layers import *
-from bert4keras3.snippets import insert_arguments
-from bert4keras3.snippets import delete_arguments
-from bert4keras3.snippets import is_string, string_matching
-from bert4keras3.snippets import orthogonally_resize
-from keras.models import Model
-import json
 
 
-class Transformer(object):
-    """模型基类
-    """
-    def __init__(
-        self,
-        vocab_size,  # 词表大小
-        hidden_size,  # 编码维度
-        num_hidden_layers,  # Transformer总层数
-        num_attention_heads,  # Attention的头数
-        intermediate_size,  # FeedForward的隐层维度
-        hidden_act,  # FeedForward隐层的激活函数
-        dropout_rate=None,  # Dropout比例
-        attention_dropout_rate=None,  # Attention矩阵的Dropout比例
-        embedding_size=None,  # 是否指定embedding_size
-        attention_head_size=None,  # Attention中V的head_size
-        attention_key_size=None,  # Attention中Q,K的head_size
-        sequence_length=None,  # 是否固定序列长度
-        keep_tokens=None,  # 要保留的词ID列表
-        compound_tokens=None,  # 扩展Embedding
-        residual_attention_scores=False,  # Attention矩阵加残差
-        ignore_invalid_weights=False,  # 允许跳过不存在的权重
-        autoresize_weights=False,  # 自动变换形状不匹配的权重
-        layers=None,  # 外部传入的Keras层
-        prefix=None,  # 层名前缀
-        name=None,  # 模型名称
-        segment_attention=False,
-        **kwargs
-    ):
-        if keep_tokens is not None:
-            vocab_size = len(keep_tokens)
-        if compound_tokens is not None:
-            vocab_size += len(compound_tokens)
-        self.vocab_size = vocab_size
-        self.segment_attention = segment_attention
-        self.hidden_size = hidden_size
-        self.num_hidden_layers = num_hidden_layers
-        self.num_attention_heads = num_attention_heads
-        self.attention_head_size = attention_head_size or hidden_size // num_attention_heads
-        self.attention_key_size = attention_key_size or self.attention_head_size
-        self.intermediate_size = intermediate_size
-        self.dropout_rate = dropout_rate or 0
-        self.attention_dropout_rate = attention_dropout_rate or 0
-        self.hidden_act = hidden_act
-        self.embedding_size = embedding_size or hidden_size
-        self.sequence_length = sequence_length
-        self.keep_tokens = keep_tokens
-        self.compound_tokens = compound_tokens
-        self.attention_bias = None
-        self.position_bias = None
-        self.attention_scores = None
-        self.residual_attention_scores = residual_attention_scores
-        self.ignore_invalid_weights = ignore_invalid_weights
-        self.autoresize_weights = autoresize_weights
-        self.layers = {} if layers is None else layers
-        self.prefix = prefix or ''
-        self.name = name
-        self.built = False
-        self.cache_position_bias = None
-        self.cache_attention_bias= None
-        self.single_head = False
-        self.is_seq2seq = False
-        self._seed_generators = []
-        self.custom_position_ids = False
-    def build(
-        self,
-        attention_caches=None,
-        layer_norm_cond=None,
-        layer_norm_cond_hidden_size=None,
-        layer_norm_cond_hidden_act=None,
-        additional_input_layers=None,
-        **kwargs
-    ):
-        """模型构建函数
-        attention_caches：为Attention的K,V的缓存序列字典，格式为
-                         {Attention层名: [K缓存, V缓存]}；
-        layer_norm_*系列参数：实现Conditional Layer Normalization时使用，
-                            用来实现以“固定长度向量”为条件的条件Bert。
-        """
-        if self.built:
-            return None
-        # Input
-        inputs = self.get_inputs()
-        self.set_inputs(inputs, additional_input_layers)
-        # Other
-        self.attention_caches = attention_caches or {}
-        self.layer_norm_conds = [
-            layer_norm_cond,
-            layer_norm_cond_hidden_size,
-            layer_norm_cond_hidden_act or 'linear',
-        ]
-        
-        outputs = self.call(inputs)
-        self.set_outputs(outputs)
-        # Model
-        self.model = Model(self.inputs, self.outputs, name=self.name)
-        self.built = True
-
-    def call(self, inputs):
-        """定义模型的执行流程
-        """
-        # Embedding
-        outputs = self.apply_embeddings(inputs)
-        # Main
-        for i in range(self.num_hidden_layers):
-            outputs = self.apply_main_layers(outputs, i)
-        # Final
-        outputs = self.apply_final_layers(outputs)
-        return outputs
-
-    def prefixed(self, name):
-        """给名字加前缀
-        """
-        if name is not None:
-            return self.prefix + name
-
-    def apply(self, inputs=None, layer=None, arguments=None, **kwargs):
-        """通过apply调用层会自动重用同名层
-        inputs: 上一层的输出；
-        layer: 要调用的层类名；
-        arguments: 传递给layer.call的参数；
-        kwargs: 传递给层初始化的参数。
-        """
-        if layer is Dropout and self.dropout_rate == 0:
-            return inputs
-
-        if layer is MultiHeadAttention and self.residual_attention_scores:
-            kwargs['return_attention_scores'] = True
-
-        arguments = arguments or {}
-        if layer is Lambda:
-            kwargs['arguments'] = arguments
-            arguments = {}
-
-        name = self.prefixed(kwargs.get('name'))
-        kwargs['name'] = name
-        if name not in self.layers:
-            layer = layer(**kwargs)
-            name = layer.name
-            self.layers[name] = layer
-
-        if inputs is None:
-            return self.layers[name]
-        else:
-            if isinstance(self.layers[name], MultiHeadAttention):
-                if name in self.attention_caches:
-                    # 如果检测到Cache的传入，那么自动在Key,Value处拼接起来
-                    k_cache, v_cache = self.attention_caches[name]
-                    k_name, v_name = name + '-Cached-Key', name + '-Cached-Value'
-                    k = Concatenate1D(name=k_name)([k_cache, inputs[1]])
-                    v = Concatenate1D(name=v_name)([v_cache, inputs[2]])
-                    inputs = inputs[:1] + [k, v] + inputs[3:]
-                if self.residual_attention_scores:
-                    # 如果使用残差Attention矩阵，则给每个Attention矩阵加上前上一层的Attention
-                    # 矩阵，这对应RealFormer设计（https://arxiv.org/abs/2012.11747）。目前
-                    # 该实现还相对粗糙，可能欠缺通用性。
-                    if self.attention_scores is not None:
-                        if arguments.get('a_bias'):
-                            a_bias = Add(name=name + '-Attention-Bias'
-                                        )([inputs[3], self.attention_scores])
-                            inputs = inputs[:3] + [a_bias] + inputs[4:]
-                        else:
-                            a_bias = self.attention_scores
-                            inputs = inputs[:3] + [a_bias] + inputs[3:]
-                        arguments['a_bias'] = True
-                    o, a = self.layers[name](inputs, **arguments)
-                    self.attention_scores = a
-                    return o
-            return self.layers[name](inputs, **arguments)
-
-    def get_inputs(self):
-        raise NotImplementedError
-
-    def apply_embeddings(self, inputs):
-        raise NotImplementedError
-
-    def apply_main_layers(self, inputs, index):
-        raise NotImplementedError
-
-    def apply_final_layers(self, inputs):
-        raise NotImplementedError
-
-    def compute_attention_bias(self, inputs=None):
-        """定义每一层的Attention Bias
-        """
-        return self.attention_bias
-
-    def compute_position_bias(self, inputs=None):
-        """定义每一层的Position Bias（一般相对位置编码用）
-        """
-        return self.position_bias
-
-    def set_inputs(self, inputs, additional_input_layers=None):
-        """设置input和inputs属性
-        """
-        if inputs is None:
-            inputs = []
-        elif not isinstance(inputs, list):
-            inputs = [inputs]
-
-        inputs = inputs[:]
-        if additional_input_layers is not None:
-            if not isinstance(additional_input_layers, list):
-                additional_input_layers = [additional_input_layers]
-            inputs.extend(additional_input_layers)
-
-        self.inputs = inputs
-        if len(inputs) > 1:
-            self.input = inputs
-        else:
-            self.input = inputs[0]
-
-    def set_outputs(self, outputs):
-        """设置output和outputs属性
-        """
-        if not isinstance(outputs, list):
-            outputs = [outputs]
-
-        outputs = outputs[:]
-        self.outputs = outputs
-        if len(outputs) > 1:
-            self.output = outputs
-        else:
-            self.output = outputs[0]
-
-    @property
-    def initializer(self):
-        """默认使用截断正态分布初始化
-        """
-        return keras.initializers.TruncatedNormal(stddev=0.02)
-
-    def simplify(self, inputs):
-        """将list中的None过滤掉
-        """
-        inputs = [i for i in inputs if i is not None]
-        if len(inputs) == 1:
-            inputs = inputs[0]
-
-        return inputs
-
-    def load_embeddings(self, embeddings):
-        """处理Embedding层权重
-        """
-        embeddings = embeddings.astype(K.floatx())  # 防止np.average报错
-
-        if self.keep_tokens is not None:
-            embeddings = embeddings[self.keep_tokens]
-
-        if self.compound_tokens is not None:
-            ext_embeddings = []
-            for item in self.compound_tokens:
-                if isinstance(item, list):
-                    item = (item, [1] * len(item))
-                ext_embeddings.append(
-                    np.average(embeddings[item[0]], 0, item[1])
-                )
-            embeddings = np.concatenate([embeddings, ext_embeddings], 0)
-
-        return embeddings
-
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        if isinstance(checkpoint, dict):
-            return checkpoint[name]
-        else:
-            return tf.train.load_variable(checkpoint, name)
-
-    def create_variable(self, name, value, dtype=None):
-        """创建一个变量
-        """
-        dtype = dtype or K.floatx()
-        return K.variable(
-            self.initializer(value.shape, dtype), dtype, name=name
-        ), value
-
-    def variable_mapping(self):
-        """构建keras层与checkpoint的变量名之间的映射表
-        """
-        return {}
-    def load_weights_from_checkpoint(self, checkpoint, mapping=None):
-        """根据mapping从checkpoint加载权重
-        """
-        mapping = mapping or self.variable_mapping()
-        mapping = {self.prefixed(k): v for k, v in mapping.items()}
-        mapping = {k: v for k, v in mapping.items() if k in self.layers}
-
-       
-        for layer, variables in mapping.items():
-            weight_value_pairs = []
-            layer = self.layers[layer]
-            weights, values = [], []
-
-            for w, v in zip(layer.trainable_weights, variables):  # 允许跳过不存在的权重
-                try:
-                    values.append(self.load_variable(checkpoint, v))
-                    weights.append(w)
-                except Exception as e:
-                    if self.ignore_invalid_weights:
-                        print('%s, but ignored.' % e.message)
-                        weights.append(w)
-                    else:
-                        raise e
-
-            for i, (w, v) in enumerate(zip(weights, values)):
-                if v is not None:
-                    w_shape, v_shape = int_shape(w), v.shape
-                    if self.autoresize_weights and w_shape != v_shape:
-                        v = orthogonally_resize(v, w_shape)
-                        if isinstance(layer, MultiHeadAttention):
-                            count = 2
-                            if layer.use_bias:
-                                count += 2
-                            if layer.attention_scale and i < count:
-                                scale = 1.0 * w_shape[-1] / v_shape[-1]
-                                v = v * scale**0.25
-                        if isinstance(layer, FeedForward):
-                            count = 1
-                            if layer.use_bias:
-                                count += 1
-                            if self.hidden_act in ['relu', 'leaky_relu']:
-                                count -= 2
-                            if i < count:
-                                v *= np.sqrt(1.0 * w_shape[-1] / v_shape[-1])
-                            else:
-                                v *= np.sqrt(1.0 * v_shape[0] / w_shape[0])
-                    weight_value_pairs.append(v)
-                else:
-                     weight_value_pairs.append(w.numpy())
-            try:
-                layer.set_weights(weight_value_pairs)
-            except:
-                if self.ignore_invalid_weights:
-                    print('%s, but ignored.' % e.message)
-                else:
-                    raise e
-            
-    def Search(self,inputs,k=1,mode='greedy'):
-        if mode=='topp':
-            return self.apply(
-                inputs=inputs,
-                layer=ToppSearch,
-                k=k,
-                end_token=self.end_token,
-                name='SearchLayer'
-            )
-        elif mode=='topk':
-            return self.apply(
-                inputs=inputs,
-                layer=TopkSearch,
-                k=k,
-                end_token=self.end_token,
-                name='SearchLayer'
-            )
-        else:
-            return self.apply(
-                inputs=inputs,
-                layer=GreedySearch,
-                k=k,
-                end_token=self.end_token,
-                name='SearchLayer'
-            )
-
-    def compute_cache_position_bias(self, inputs=None,self_cache_update_index=None,index=None):
-        return None
-
-    def apply_main_cache_layers(self, inputs, index,self_cache_update_index,
-                                cross_cache_update_index=None,
-                                attention_mask=None,position_bias=None,
-            
-                                ):
-        raise('this model not support cache model')
-    def get_cache_inputs(self,lengths:list):
-        raise('this model not support cache model')
-    def get_custom_position_ids(self):
-        return self.custom_position_ids
-class LM_Mask(object):
-    """定义下三角Attention Mask（语言模型用）
-    """
-        
-    def compute_attention_bias(self, inputs=None):
-        """通过idxs序列的比较来得到对应的mask
-        """
-        if self.attention_bias is None:
-
-            def lm_mask(s):
-                seq_len = ops.shape(s)[1]
-                idxs = ops.arange(0, seq_len)
-                mask = idxs[None, :] <= idxs[:, None]
-                return mask
-
-            self.attention_bias = self.apply(
-                inputs=self.inputs[0],
-                dtype='float32',
-                layer=Lambda,
-                function=lm_mask,
-                name='Attention-Mask'
-            )
-
-        return self.attention_bias
-    def compute_cache_attention_bias(self, inputs=None,key=0,index=0):
-        if self.cache_attention_bias==None:
-            self.cache_attention_bias=self.apply(
-                inputs=inputs[key],
-                name='Attention-Mask'
-            )
-        else:
-            return self.apply(
-                inputs=self.cache_attention_bias,
-                layer=TakeLayer,
-                arguments={'index': index},
-                axis=0,
-                name='TakeLayer2'
-            )
-    def initial_cache(self,inputs):
-        caches=[]
-        class Initial_cache(Layer):
-            def __init__(self, attention_key_size,num_attention_heads,single_head=False, **kwargs):
-                super(Initial_cache, self).__init__(**kwargs)
-                self.single_head =single_head
-                self.attention_key_size=attention_key_size
-                self.num_attention_heads=num_attention_heads
-            def get_config(self):
-                config = {
-                    'single_head': self.single_head,
-                    'num_attention_heads':self.num_attention_heads,
-                    'attention_key_size':self.attention_key_size
-                }
-                base_config = super(Initial_cache, self).get_config()
-                return dict(list(base_config.items()) + list(config.items()))
-            def call(self,inputs, **kwargs):
-                caches=[]
-                for t in inputs:
-                    if self.single_head:
-                        cache_shape=[ops.shape(t)[0],2,ops.shape(t)[1],self.attention_key_size] 
-                    else:
-                        cache_shape=[ops.shape(t)[0],2,ops.shape(t)[1],self.num_attention_heads,self.attention_key_size]
-                    caches.append(ops.zeros(cache_shape,dtype=t.dtype))
-                return caches
-            def compute_output_shape(self, input_shape):
-                shapes=[]
-                for t in input_shape:
-                    if self.single_head:
-                        shapes.append([t[0],2,t[1],self.attention_key_size])      
-                    else:
-                        shapes.append([t[0],2,t[1],self.num_attention_heads,self.attention_key_size])   
-                return shapes
-        for _ in range(self.num_hidden_layers):
-            caches.extend(self.apply(
-                inputs=inputs,
-                layer=Initial_cache,
-                single_head=self.single_head,
-                num_attention_heads = self.num_attention_heads,
-                attention_key_size = self.attention_key_size,
-                name='Initial_caches'
-            ))
-        return caches
-    def slice_inputs(self,inputs,key,index):
-        return ops.expand_dims(ops.take(inputs[key],index,axis=1),1)
-    def get_new_inputs(self,inputs,key,xs,index=None):
-        return inputs[:key]+[xs]+inputs[key+1:]
-    def cache_call(self,inputs:list,input_lengths:list,end_token,
-                   search_mode='greedy',k=1,progress_print=True,index_bias=0):
-        old_flag = self.custom_position_ids
-        if self.is_seq2seq:
-            caches = self.initial_cache([inputs[1],inputs[0]])
-            key = 1
-        else:
-            caches = self.initial_cache(inputs[:1])
-            key = 0
-        x = inputs[key]
-        
-        class start_index(keras.Layer):
-            def call(self,x):
-                z = x!=0
-                if index_bias>0:
-                    t = ops.ones([ops.shape(z)[0],index_bias],dtype=z.dtype)
-                    z = ops.slice_update(z,[0,0],t)
-                return ops.max(ops.sum(z,-1))-1
-        
-        
-        length = input_lengths[key]
-        self.cache_attention_bias=None
-        self.cache_position_bias=None
-        self.compute_cache_attention_bias(inputs,key,index=0)
-        self.compute_cache_position_bias(inputs)
-        self.end_token = end_token
-        #initial inputs and cache
-
-        z = self.apply_embeddings(inputs)
-
-        if not isinstance(z,list):
-            z = [z]
-        j = len(caches)//self.num_hidden_layers
-        
-        for index in range(self.num_hidden_layers):
-            layer_caches = caches[index*j:index*j+j]
-            out=self.apply_main_cache_layers(z+[layer_caches], index,self_cache_update_index=ops.zeros([],'int32'),
-                                        cross_cache_update_index=ops.zeros([],'int32'),
-                                        attention_mask=self.cache_attention_bias,
-                                        position_bias=self.cache_position_bias)
-            z,cache = out[:-1],out[-1]
-            
-            caches[index*j:index*j+j]=cache
-        
-        
-        
-        index = self.apply(
-            inputs=x,
-            layer=start_index,
-            name='start_index'
-        )
-        
-        def cond(inputs, caches, index , flags):
-            cond1 = ops.less(index,length-1)
-            cond2 = ops.logical_not(ops.all(ops.equal(inputs[key][:,index],end_token),-1))
-            return ops.logical_and(cond1,cond2)
-        
-        def body(inputs, caches, index , flags):
-            if progress_print:
-                
-                print('\r',index,end='')
-            xs = self.slice_inputs(inputs,key,index)
-            self.custom_position_ids = self.get_custom_position_ids()
-            new_inputs = self.get_new_inputs(inputs,key,xs,index)
-            if self.custom_position_ids:
-                new_inputs += [ops.reshape(index,[-1,1])]
-            z = self.apply_embeddings(new_inputs)
-            
-            if not isinstance(z,list):
-                z = [z]
-            attention_mask = self.compute_cache_attention_bias(index=index)
-            position_bias = self.compute_cache_position_bias(self_cache_update_index = index) 
-            
-            for i in range(self.num_hidden_layers):
-                
-                layer_caches = caches[i*j:i*j+j]
-                out=self.apply_main_cache_layers(z+[layer_caches], i,self_cache_update_index=index,
-                                            cross_cache_update_index=None,
-                                            attention_mask=attention_mask,
-                                            position_bias=position_bias)
-                
-                z,cache = out[:-1],out[-1]
-                
-                caches[i*j:i*j+j]=cache
-            
-
-            o = self.apply_final_layers(z)
-            
-            index += 1
-            search_in = [o,index,inputs[key],flags]
-            inputs[key],flags = self.Search(search_in,k=k,mode=search_mode)
-            return (inputs, caches, index , flags)
-        num_hidden_layers = self.num_hidden_layers
-        class WhileLayer(keras.Layer):
-            def call(self, x):
-                inputs, caches, index =  x[:]
-                flags = ops.ones([ops.shape(caches[0])[0],1],dtype='bool')
-                if backlib=='torch':
-                    while cond(inputs, caches, index , flags):
-                        inputs, caches, index , flags = body(inputs, caches, index , flags)
-                    return (inputs, caches, index)
-                outs=ops.while_loop(
-                    cond,
-                    body,
-                    loop_vars=(inputs, caches, index , flags),
-                    maximum_iterations=length-index                                                                                                                                                                                                                                                                                                                                                       ,
-                )
-                if progress_print:
-                    print('\n')
-                return outs[:3]
-            def compute_output_shape(self, input_shape):
-                return input_shape
-        out=self.apply(
-            inputs=(inputs, caches, index),
-            layer=WhileLayer,
-            name='WhileLayer'
-        )
-        self.custom_position_ids = old_flag
-        return ops.cast(out[0][key],'int32')
-    def build_cache_model(self,input_lengths:list,end_token,
-                          search_mode='greedy',k=1,progress_print=False,index_bias=0):
-        
-        inputs=self.get_cache_inputs(input_lengths)
-        
-        out = self.cache_call(inputs=inputs,input_lengths=input_lengths,end_token=end_token,
-                       search_mode=search_mode,k=k,progress_print=progress_print,index_bias=index_bias)
-        model = keras.Model(inputs,out)
-        inputs = []
-        for modelin in model.inputs: 
-            shape=keras.ops.shape(modelin)
-            shape=[1 if t==None else t for t in shape]
-            inputs.append(ops.convert_to_tensor(np.ones(shape),modelin.dtype))
-        self.cache_call(inputs=inputs,input_lengths=input_lengths,end_token=end_token,
-                       search_mode=search_mode,k=k,progress_print=progress_print,index_bias=index_bias)
-        
-        return model
-class UniLM_Mask(LM_Mask):
-    """定义UniLM的Attention Mask（Seq2Seq模型用）
-    其中source和target的分区，由segment_ids来表示。
-    UniLM: https://arxiv.org/abs/1905.03197
-    """
-    def compute_attention_bias(self, inputs=None):
-        """通过idxs序列的比较来得到对应的mask
-        """
-        if self.attention_bias is None:
-
-            if self.segment_attention:
-                def unilm_mask(s):
-                    mask = s[:, None, :] <= s[:, :, None]
-                    return mask
-            else:
-                def unilm_mask(s):
-                    idxs = ops.cumsum(s, axis=1)
-                    mask = idxs[:, None, :] <= idxs[:, :, None]
-                    return mask
-            
-            self.attention_bias = self.apply(
-                inputs=self.inputs[1],
-                layer=Lambda,
-                function=unilm_mask,
-                dtype='float32',
-                name='Attention-Mask'
-            )
-
-        return self.attention_bias
-    def slice_inputs(self,inputs,key,index):
-        def take(inputs,key,index):
-            return ops.expand_dims(ops.take(inputs[key],index,axis=1),1)
-        return [take(inputs,key,index),take(inputs,key+1,index)]
-    def get_new_inputs(self,inputs,key,xs,index=None):
-        if self.custom_position_ids:
-            return inputs[:key]+xs+[ops.expand_dims(index,0)]+inputs[key+2:]
-        return inputs[:key]+xs+inputs[key+2:]
-    def compute_cache_attention_bias(self, inputs=None,key=0,index=0):
-        
-        if self.cache_attention_bias==None:
-            self.cache_attention_bias=self.apply(
-                inputs=inputs[key+1],
-                name='Attention-Mask'
-            )
-        else:
-            return self.apply(
-                inputs=self.cache_attention_bias,
-                layer=TakeLayer,
-                axis=1,
-                arguments={'index': index},
-                name='TakeLayer'
-            )
-
-            def unilm_mask(s):
-                idxs = ops.cumsum(s, axis=1)
-                mask = idxs[:, None, :] <= idxs[:, :, None]
-                return mask
-
-            self.attention_bias = self.apply(
-                inputs=self.inputs[1],
-                layer=Lambda,
-                function=unilm_mask,
-                name='Attention-Mask'
-            )
-
-        return self.attention_bias
-    def slice_inputs(self,inputs,key,index):
-        def take(inputs,key,index):
-            return ops.expand_dims(ops.take(inputs[key],index,axis=1),1)
-        return [take(inputs,key,index),take(inputs,key+1,index)]
-    def get_new_inputs(self,inputs,key,xs,index=None):
-        if self.custom_position_ids:
-            return inputs[:key]+xs+[ops.expand_dims(index,0)]+inputs[key+2:]
-        return inputs[:key]+xs+inputs[key+2:]
-    def compute_cache_attention_bias(self, inputs=None,key=0,index=0):
-        
-        if self.cache_attention_bias==None:
-            self.cache_attention_bias=self.apply(
-                inputs=inputs[key+1],
-                name='Attention-Mask'
-            )
-        else:
-            return self.apply(
-                inputs=self.cache_attention_bias,
-                layer=TakeLayer,
-                axis=1,
-                arguments={'index': index},
-                name='TakeLayer'
-            )
-class BERT(Transformer):
-    """构建BERT模型
-    """
-    def __init__(
-        self,
-        max_position,  # 序列最大长度
-        segment_vocab_size=2,  # segment总数目
-        with_pool=False,  # 是否包含Pool部分
-        with_nsp=False,  # 是否包含NSP部分
-        with_mlm=False,  # 是否包含MLM部分
-        hierarchical_position=None,  # 是否层次分解位置编码
-        custom_position_ids=False,  # 是否自行传入位置id
-        shared_segment_embeddings=False,  # 若True，则segment跟token共用embedding
-        **kwargs  # 其余参数
-    ):
-        super(BERT, self).__init__(**kwargs)
-        self.max_position = max_position
-        self.segment_vocab_size = segment_vocab_size
-        self.with_pool = with_pool
-        self.with_nsp = with_nsp
-        self.with_mlm = with_mlm
-        self.hierarchical_position = hierarchical_position
-        self.custom_position_ids = custom_position_ids
-        self.shared_segment_embeddings = shared_segment_embeddings
-        if self.with_nsp and not self.with_pool:
-            self.with_pool = True
-    def get_custom_position_ids(self):
-        return True
-    def get_inputs(self):
-        """BERT的输入是token_ids和segment_ids
-        （但允许自行传入位置id，以实现一些特殊需求）
-        """
-        x_in = self.apply(
-            layer=Input, shape=(self.sequence_length,), name='Input-Token'
-        )
-        inputs = [x_in]
-
-        if self.segment_vocab_size > 0:
-            s_in = self.apply(
-                layer=Input,
-                shape=(self.sequence_length,),
-                name='Input-Segment'
-            )
-            inputs.append(s_in)
-
-        if self.custom_position_ids:
-            p_in = self.apply(
-                layer=Input,
-                shape=(self.sequence_length,),
-                name='Input-Position'
-            )
-            inputs.append(p_in)
-
-        return inputs
-    
-    def apply_main_cache_layers(self, inputs, index,self_cache_update_index,
-                                cross_cache_update_index=None,
-                                attention_mask=None,position_bias=None,
-            
-                                ):
-        x,caches = inputs[:]
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-
-        # Self Attention
-        xi, x, arguments = x, [x, x, x,attention_mask,caches[0],self_cache_update_index], {'a_bias': True,'cache_update_index':True,'use_cache':True,}
-        x,cache = self.apply(
-            inputs=x,
-            arguments=arguments,
-            name=attention_name
-        )
-        caches[0] = cache
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return [x,caches]
-    def get_cache_inputs(self,lengths:list):
-        x_in = self.apply(
-            layer=Input, shape=[lengths[1]], name='Input-Token-cache-'+str(lengths[1])
-        )
-        inputs = [x_in]
-
-        if self.segment_vocab_size > 0:
-            s_in = self.apply(
-                layer=Input,
-                shape=[lengths[1]],
-                name='Input-Segment-cache-'+str(lengths[1])
-            )
-            inputs.append(s_in)
-        
-        return inputs
-
-    def apply_embeddings(self, inputs):
-        """BERT的embedding是token、position、segment三者embedding之和
-        """
-        inputs = inputs[:]
-        x = inputs.pop(0)
-        if self.segment_vocab_size > 0:
-            s = inputs.pop(0)
-        if self.custom_position_ids:
-            p = inputs.pop(0)
-        else:
-            p = None
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        if self.segment_vocab_size > 0:
-            if self.shared_segment_embeddings:
-                name = 'Embedding-Token'
-            else:
-                name = 'Embedding-Segment'
-            s = self.apply(
-                inputs=s,
-                layer=Embedding,
-                input_dim=self.segment_vocab_size,
-                output_dim=self.embedding_size,
-                embeddings_initializer=self.initializer,
-                name=name
-            )
-            x = self.apply(
-                inputs=[x, s], layer=Add, name='Embedding-Token-Segment'
-            )
-        x = self.apply(
-            inputs=self.simplify([x, p]),
-            layer=PositionEmbedding,
-            input_dim=self.max_position,
-            output_dim=self.embedding_size,
-            merge_mode='add',
-            hierarchical=self.hierarchical_position,
-            embeddings_initializer=self.initializer,
-            custom_position_ids=self.custom_position_ids,
-            name='Embedding-Position'
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-12,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Embedding-Norm'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Embedding-Dropout'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """BERT的主体是基于Self-Attention的模块
-        顺序：Att --> Add --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-
-        # Self Attention
-        xi, x, arguments = x, [x, x, x], {'a_bias': None}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.append(attention_mask)
-
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-12,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-12,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return x
-
-    def apply_final_layers(self, inputs):
-        """根据剩余参数决定输出
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-        if isinstance(x,list):
-            outputs = x
-        else:
-            outputs = [x]
-
-        if self.with_pool:
-            # Pooler部分（提取CLS向量）
-            x = outputs[0]
-            x = self.apply(
-                inputs=x,
-                layer=Lambda,
-                function=lambda x: x[:, 0],
-                name='Pooler'
-            )
-            pool_activation = 'tanh' if self.with_pool is True else self.with_pool
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                activation=pool_activation,
-                kernel_initializer=self.initializer,
-                name='Pooler-Dense'
-            )
-            if self.with_nsp:
-                # Next Sentence Prediction部分
-                x = self.apply(
-                    inputs=x,
-                    layer=Dense,
-                    units=2,
-                    activation='softmax',
-                    kernel_initializer=self.initializer,
-                    name='NSP-Proba'
-                )
-            outputs.append(x)
-
-        if self.with_mlm:
-            # Masked Language Model部分
-            x = outputs[0]
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.embedding_size,
-                activation=self.hidden_act,
-                kernel_initializer=self.initializer,
-                name='MLM-Dense'
-            )
-            x = self.apply(
-                inputs=self.simplify([x, z]),
-                layer=LayerNormalization,
-                epsilon=1e-12,
-                conditional=(z is not None),
-                hidden_units=self.layer_norm_conds[1],
-                hidden_activation=self.layer_norm_conds[2],
-                hidden_initializer=self.initializer,
-                name='MLM-Norm'
-            )
-            x = self.apply(
-                inputs=x,
-                layer=Embedding,
-                arguments={'mode': 'dense'},
-                name='Embedding-Token'
-            )
-            x = self.apply(
-                inputs=x, layer=ScaleOffset, scale=False, name='MLM-Bias'
-            )
-            mlm_activation = 'softmax' if self.with_mlm is True else self.with_mlm
-            x = self.apply(
-                inputs=x,
-                layer=Activation,
-                activation=mlm_activation,
-                name='MLM-Activation'
-            )
-            outputs.append(x)
-
-        if len(outputs) == 1:
-            outputs = outputs[0]
-        elif len(outputs) == 2:
-            outputs = outputs[1]
-        else:
-            outputs = outputs[1:]
-
-        return outputs
-
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        variable = super(BERT, self).load_variable(checkpoint, name)
-        if name in [
-            'bert/embeddings/word_embeddings',
-            'cls/predictions/output_bias',
-        ]:
-            return self.load_embeddings(variable)
-        elif name == 'cls/seq_relationship/output_weights':
-            return variable.T
-        else:
-            return variable
-
-    def create_variable(self, name, value, dtype=None):
-        """在tensorflow中创建一个变量
-        """
-        if name == 'cls/seq_relationship/output_weights':
-            value = value.T
-        return super(BERT, self).create_variable(name, value, dtype)
-
-    def variable_mapping(self):
-        """映射到官方BERT权重格式
-        """
-        mapping = {
-            'Embedding-Token': ['bert/embeddings/word_embeddings'],
-            'Embedding-Segment': ['bert/embeddings/token_type_embeddings'],
-            'Embedding-Position': ['bert/embeddings/position_embeddings'],
-            'Embedding-Norm': [
-                'bert/embeddings/LayerNorm/beta',
-                'bert/embeddings/LayerNorm/gamma',
-            ],
-            'Embedding-Mapping': [
-                'bert/encoder/embedding_hidden_mapping_in/kernel',
-                'bert/encoder/embedding_hidden_mapping_in/bias',
-            ],
-            'Pooler-Dense': [
-                'bert/pooler/dense/kernel',
-                'bert/pooler/dense/bias',
-            ],
-            'NSP-Proba': [
-                'cls/seq_relationship/output_weights',
-                'cls/seq_relationship/output_bias',
-            ],
-            'MLM-Dense': [
-                'cls/predictions/transform/dense/kernel',
-                'cls/predictions/transform/dense/bias',
-            ],
-            'MLM-Norm': [
-                'cls/predictions/transform/LayerNorm/beta',
-                'cls/predictions/transform/LayerNorm/gamma',
-            ],
-            'MLM-Bias': ['cls/predictions/output_bias'],
-        }
-
-        for i in range(self.num_hidden_layers):
-            prefix = 'bert/encoder/layer_%d/' % i
-            mapping.update({
-                'Transformer-%d-MultiHeadSelfAttention' % i: [
-                    prefix + 'attention/self/query/kernel',
-                    prefix + 'attention/self/query/bias',
-                    prefix + 'attention/self/key/kernel',
-                    prefix + 'attention/self/key/bias',
-                    prefix + 'attention/self/value/kernel',
-                    prefix + 'attention/self/value/bias',
-                    prefix + 'attention/output/dense/kernel',
-                    prefix + 'attention/output/dense/bias',
-                ],
-                'Transformer-%d-MultiHeadSelfAttention-Norm' % i: [
-                    prefix + 'attention/output/LayerNorm/beta',
-                    prefix + 'attention/output/LayerNorm/gamma',
-                ],
-                'Transformer-%d-FeedForward' % i: [
-                    prefix + 'intermediate/dense/kernel',
-                    prefix + 'intermediate/dense/bias',
-                    prefix + 'output/dense/kernel',
-                    prefix + 'output/dense/bias',
-                ],
-                'Transformer-%d-FeedForward-Norm' % i: [
-                    prefix + 'output/LayerNorm/beta',
-                    prefix + 'output/LayerNorm/gamma',
-                ],
-            })
-
-        return mapping
-
-
-class ALBERT(BERT):
-    """构建ALBERT模型
-    """
-    def apply_main_layers(self, inputs, index):
-        """ALBERT的主体是基于Self-Attention的模块
-        顺序：Att --> Add --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-MultiHeadSelfAttention'
-        feed_forward_name = 'Transformer-FeedForward'
-        attention_mask = self.compute_attention_bias(index)
-
-        # Self Attention
-        xi, x, arguments = x, [x, x, x], {'a_bias': None}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.append(attention_mask)
-
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return x
-
-    def variable_mapping(self):
-        """映射到官方ALBERT权重格式
-        """
-        mapping = super(ALBERT, self).variable_mapping()
-
-        prefix = 'bert/encoder/transformer/group_0/inner_group_0/'
-        mapping.update({
-            'Transformer-MultiHeadSelfAttention': [
-                prefix + 'attention_1/self/query/kernel',
-                prefix + 'attention_1/self/query/bias',
-                prefix + 'attention_1/self/key/kernel',
-                prefix + 'attention_1/self/key/bias',
-                prefix + 'attention_1/self/value/kernel',
-                prefix + 'attention_1/self/value/bias',
-                prefix + 'attention_1/output/dense/kernel',
-                prefix + 'attention_1/output/dense/bias',
-            ],
-            'Transformer-MultiHeadSelfAttention-Norm': [
-                prefix + 'LayerNorm/beta',
-                prefix + 'LayerNorm/gamma',
-            ],
-            'Transformer-FeedForward': [
-                prefix + 'ffn_1/intermediate/dense/kernel',
-                prefix + 'ffn_1/intermediate/dense/bias',
-                prefix + 'ffn_1/intermediate/output/dense/kernel',
-                prefix + 'ffn_1/intermediate/output/dense/bias',
-            ],
-            'Transformer-FeedForward-Norm': [
-                prefix + 'LayerNorm_1/beta',
-                prefix + 'LayerNorm_1/gamma',
-            ],
-        })
-
-        return mapping
-
-
-class ALBERT_Unshared(BERT):
-    """解开ALBERT共享约束，当成BERT用
-    """
-    def variable_mapping(self):
-        """映射到官方ALBERT权重格式
-        """
-        mapping = super(ALBERT_Unshared, self).variable_mapping()
-
-        prefix = 'bert/encoder/transformer/group_0/inner_group_0/'
-        for i in range(self.num_hidden_layers):
-            mapping.update({
-                'Transformer-%d-MultiHeadSelfAttention' % i: [
-                    prefix + 'attention_1/self/query/kernel',
-                    prefix + 'attention_1/self/query/bias',
-                    prefix + 'attention_1/self/key/kernel',
-                    prefix + 'attention_1/self/key/bias',
-                    prefix + 'attention_1/self/value/kernel',
-                    prefix + 'attention_1/self/value/bias',
-                    prefix + 'attention_1/output/dense/kernel',
-                    prefix + 'attention_1/output/dense/bias',
-                ],
-                'Transformer-%d-MultiHeadSelfAttention-Norm' % i: [
-                    prefix + 'LayerNorm/beta',
-                    prefix + 'LayerNorm/gamma',
-                ],
-                'Transformer-%d-FeedForward' % i: [
-                    prefix + 'ffn_1/intermediate/dense/kernel',
-                    prefix + 'ffn_1/intermediate/dense/bias',
-                    prefix + 'ffn_1/intermediate/output/dense/kernel',
-                    prefix + 'ffn_1/intermediate/output/dense/bias',
-                ],
-                'Transformer-%d-FeedForward-Norm' % i: [
-                    prefix + 'LayerNorm_1/beta',
-                    prefix + 'LayerNorm_1/gamma',
-                ],
-            })
-
-        return mapping
-
-
-class NEZHA(BERT):
-    """华为推出的NAZHA模型
-    链接：https://arxiv.org/abs/1909.00204
-    """
-    def apply_embeddings(self, inputs):
-        """NEZHA的embedding是token、segment两者embedding之和
-        """
-        inputs = inputs[:]
-        x = inputs.pop(0)
-        if self.segment_vocab_size > 0:
-            s = inputs.pop(0)
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        if self.segment_vocab_size > 0:
-            if self.shared_segment_embeddings:
-                name = 'Embedding-Token'
-            else:
-                name = 'Embedding-Segment'
-            s = self.apply(
-                inputs=s,
-                layer=Embedding,
-                input_dim=self.segment_vocab_size,
-                output_dim=self.embedding_size,
-                embeddings_initializer=self.initializer,
-                name=name
-            )
-            x = self.apply(
-                inputs=[x, s], layer=Add, name='Embedding-Token-Segment'
-            )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Embedding-Norm'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Embedding-Dropout'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """NEZHA的主体是基于Self-Attention的模块
-        顺序：Att --> Add --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias(x)
-
-        # Self Attention
-        xi, x = x, [x, x, x, position_bias]
-        arguments = {'a_bias': None, 'p_bias': 'typical_relative'}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.insert(3, attention_mask)
-
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return x
-
-    def compute_position_bias(self, inputs=None):
-        """经典相对位置编码
-        """
-        if self.position_bias is None:
-
-            x = inputs
-            self.position_bias = self.apply(
-                inputs=[x, x],
-                layer=RelativePositionEmbedding,
-                input_dim=2 * 64 + 1,
-                output_dim=self.attention_key_size,
-                embeddings_initializer='Sinusoidal',
-                name='Embedding-Relative-Position',
-                trainable=False
-            )
-
-        return self.position_bias
-
-
-class RoFormer(NEZHA):
-    """旋转式位置编码的BERT模型
-    链接：https://kexue.fm/archives/8265
-    """
-    def compute_cache_position_bias(self, inputs=None,self_cache_update_index=None,index=None):
-        if self.cache_position_bias is None:
-
-            self.cache_position_bias =self.apply(
-                inputs=inputs[0],
-                name='Embedding-Rotary-Position'
-            )
-        if inputs!=None:
-            return None
-        self.length_cache_position_bias = self.apply(
-            inputs=self.cache_position_bias,
-            layer=TakeLayer,
-            axis=1,
-            arguments={'index': self_cache_update_index},
-            name='TakeLayer'
-        )
-        
-        return self.length_cache_position_bias
-
-    def apply_main_cache_layers(self, inputs, index,self_cache_update_index,
-                                cross_cache_update_index=None,
-                                attention_mask=None,position_bias=None,
-            
-                                ):
-        x,caches = inputs[:]
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-
-        # Self Attention
-        xi, x  = x, [x, x, x,attention_mask, position_bias,caches[0],self_cache_update_index]
-        arguments = {'a_bias': True,'cache_update_index':True,'use_cache':True,'p_bias': 'rotary'}
-        x,cache = self.apply(
-            inputs=x,
-            arguments=arguments,
-            name=attention_name
-        )
-        caches[0] = cache
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return [x,caches]
-    def apply_main_layers(self, inputs, index):
-        """RoFormer的主体是基于Self-Attention的模块
-        顺序：Att --> Add --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias(x)
-
-        # Self Attention
-        xi, x = x, [x, x, x, position_bias]
-        arguments = {'a_bias': None, 'p_bias': 'rotary'}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.insert(3, attention_mask)
-
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return x
-
-    def compute_position_bias(self, inputs=None):
-        """Sinusoidal位置编码（直接返回）
-        """
-        if self.position_bias is None:
-
-            if self.custom_position_ids:
-                x = [inputs, self.inputs[2]]
-            else:
-                x = inputs
-
-            self.position_bias = self.apply(
-                inputs=x,
-                layer=SinusoidalPositionEmbedding,
-                output_dim=self.attention_key_size,
-                merge_mode='zero',
-                custom_position_ids=self.custom_position_ids,
-                name='Embedding-Rotary-Position'
-            )
-
-        return self.position_bias
-
-
-class RoFormerV2(RoFormer):
-    """RoFormerV2
-    改动：去掉bias，简化Norm，优化初始化等。
-    """
-    def initializer(self, shape, dtype=None, order=2, gain=1.0):
-        """使用截断正态分布初始化
-        """
-        if shape[0] > 10000 or shape[0] < 10:
-            hidden_size = shape[1]
-        else:
-            hidden_size = shape[0]
-        gain *= self.num_hidden_layers**(-1. / order)
-        stddev = 1.13684723 / hidden_size**0.5 * gain
-        return keras.initializers.TruncatedNormal(stddev=stddev)(shape)
-
-    def apply_embeddings(self, inputs):
-        """RoFormerV2的embedding是token、segment两者embedding之和
-        """
-        inputs = inputs[:]
-        x = inputs.pop(0)
-        if self.segment_vocab_size > 0:
-            s = inputs.pop(0)
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        if self.segment_vocab_size > 0:
-            if self.shared_segment_embeddings:
-                name = 'Embedding-Token'
-            else:
-                name = 'Embedding-Segment'
-            s = self.apply(
-                inputs=s,
-                layer=Embedding,
-                input_dim=self.segment_vocab_size,
-                output_dim=self.embedding_size,
-                embeddings_initializer=self.initializer,
-                name=name
-            )
-            x = self.apply(
-                inputs=[x, s], layer=Add, name='Embedding-Token-Segment'
-            )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Embedding-Dropout'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=LayerNormalization,
-            zero_mean=False,
-            scale=False,
-            offset=False,
-            name='Embedding-Norm'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                use_bias=False,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """RoFormerV2的主体是基于Self-Attention的模块
-        顺序：Att  --> Add --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias(x)
-
-        # Self Attention
-        xi = x
-        x = [x, x, x, position_bias]
-        arguments = {'a_bias': None, 'p_bias': 'rotary'}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.insert(3, attention_mask)
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            use_bias=False,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=LayerNormalization,
-            zero_mean=False,
-            scale=False,
-            offset=False,
-            name='%s-Norm' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            use_bias=False,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=LayerNormalization,
-            zero_mean=False,
-            scale=False,
-            offset=False,
-            name='%s-Norm' % feed_forward_name
-        )
-
-        return x
-
-    def apply_final_layers(self, inputs):
-        """剩余部分
-        """
-        x = inputs
-
-        if self.with_mlm:
-            # 预测token概率部分
-            if self.embedding_size != self.hidden_size:
-                x = self.apply(
-                    inputs=x,
-                    layer=Dense,
-                    units=self.embedding_size,
-                    use_bias=False,
-                    kernel_initializer=self.initializer,
-                    name='Output-Mapping'
-                )
-            x = self.apply(
-                inputs=x,
-                layer=Dropout,
-                rate=self.dropout_rate,
-                name='Output-MLM-Dropout'
-            )
-            mlm_activation = 'softmax' if self.with_mlm is True else self.with_mlm
-            x = self.apply(
-                inputs=x,
-                layer=Embedding,
-                arguments={'mode': 'dense'},
-                name='Embedding-Token'
-            )
-            x = self.apply(
-                inputs=x,
-                layer=Activation,
-                activation=mlm_activation,
-                name='Output-MLM-Activation'
-            )
-
-        return x
-
-    def variable_mapping(self):
-        """删掉部分权重映射
-        """
-        mapping = super(RoFormerV2, self).variable_mapping()
-
-        for k, v in mapping.items():
-            v = [
-                i for i in v
-                if not string_matching(i, ['beta', 'gamma', 'bias'])
-            ]
-            mapping[k] = v
-
-        return mapping
-
-
-class ELECTRA(BERT):
-    """Google推出的ELECTRA模型
-    链接：https://arxiv.org/abs/2003.10555
-    """
-    @insert_arguments(with_discriminator=False)
-    @delete_arguments('with_pool', 'with_mlm')
-    def __init__(
-        self,
-        max_position,  # 序列最大长度
-        **kwargs  # 其余参数
-    ):
-        super(ELECTRA, self).__init__(max_position, **kwargs)
-
-    def apply_final_layers(self, inputs):
-        x = inputs
-
-        if self.with_discriminator:
-            if self.with_discriminator is True:
-                final_activation = 'sigmoid'
-            else:
-                final_activation = self.with_discriminator
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                activation=self.hidden_act,
-                kernel_initializer=self.initializer,
-                name='Discriminator-Dense'
-            )
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=1,
-                activation=final_activation,
-                kernel_initializer=self.initializer,
-                name='Discriminator-Prediction'
-            )
-
-        return x
-
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        variable = super(ELECTRA, self).load_variable(checkpoint, name)
-        if name == 'electra/embeddings/word_embeddings':
-            return self.load_embeddings(variable)
-        else:
-            return variable
-
-    def variable_mapping(self):
-        mapping = super(ELECTRA, self).variable_mapping()
-        mapping['Embedding-Mapping'] = [
-            'electra/embeddings_project/kernel',
-            'electra/embeddings_project/bias',
-        ]
-        mapping = {
-            k: [i.replace('bert/', 'electra/') for i in v]
-            for k, v in mapping.items()
-        }
-        mapping['Discriminator-Dense'] = [
-            'discriminator_predictions/dense/kernel',
-            'discriminator_predictions/dense/bias',
-        ]
-        mapping['Discriminator-Prediction'] = [
-            'discriminator_predictions/dense_1/kernel',
-            'discriminator_predictions/dense_1/bias',
-        ]
-        return mapping
-
-
-class GPT(LM_Mask, BERT):
-    """构建GPT模型
-    链接：https://github.com/openai/finetune-transformer-lm
-    """
-    @insert_arguments(final_activation='softmax')
-    @delete_arguments('with_pool', 'with_mlm')
-    def __init__(self, **kwargs):
-        super(GPT, self).__init__(**kwargs)
-
-    def apply_embeddings(self, inputs):
-        """GPT的embedding是token、position、segment三者embedding之和
-        跟BERT的主要区别是三者相加之后没有加LayerNormalization层。
-        """
-        inputs = inputs[:]
-        x = inputs.pop(0)
-        if self.segment_vocab_size > 0:
-            s = inputs.pop(0)
-        if self.custom_position_ids:
-            p = inputs.pop(0)
-        else:
-            p = None
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        if self.segment_vocab_size > 0:
-            if self.shared_segment_embeddings:
-                name = 'Embedding-Token'
-            else:
-                name = 'Embedding-Segment'
-            s = self.apply(
-                inputs=s,
-                layer=Embedding,
-                input_dim=self.segment_vocab_size,
-                output_dim=self.embedding_size,
-                embeddings_initializer=self.initializer,
-                name=name
-            )
-            x = self.apply(
-                inputs=[x, s], layer=Add, name='Embedding-Token-Segment'
-            )
-        x = self.apply(
-            inputs=self.simplify([x, p]),
-            layer=PositionEmbedding,
-            input_dim=self.max_position,
-            output_dim=self.embedding_size,
-            merge_mode='add',
-            hierarchical=self.hierarchical_position,
-            embeddings_initializer=self.initializer,
-            custom_position_ids=self.custom_position_ids,
-            name='Embedding-Position'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Embedding-Dropout'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_final_layers(self, inputs):
-        """剩余部分
-        """
-        x = inputs
-
-        # Language Model部分
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            arguments={'mode': 'dense'},
-            name='Embedding-Token'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Activation,
-            activation=self.final_activation,
-            name='LM-Activation'
-        )
-
-        return x
-
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        variable = super(GPT, self).load_variable(checkpoint, name)
-        if name == 'gpt/embeddings/word_embeddings':
-            return self.load_embeddings(variable)
-        else:
-            return variable
-
-    def variable_mapping(self):
-        """映射到TF版GPT权重格式
-        """
-        mapping = super(GPT, self).variable_mapping()
-        mapping = {
-            k: [
-                i.replace('bert/', 'gpt/').replace('encoder', 'transformer')
-                for i in v
-            ]
-            for k, v in mapping.items()
-        }
-        return mapping
-
-
-class GPT2(GPT):
-    """构建GPT2模型
-    链接: https://github.com/openai/gpt-2
-    """
-    def get_inputs(self):
-        """GPT2的输入是token_ids
-        """
-        x_in = self.apply(
-            layer=Input, shape=(self.sequence_length,), name='Input-Token'
-        )
-        return x_in
-
-    def apply_embeddings(self, inputs):
-        """GPT2的embedding是token、position两者embedding之和
-        """
-        x = inputs
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=PositionEmbedding,
-            input_dim=self.max_position,
-            output_dim=self.embedding_size,
-            merge_mode='add',
-            hierarchical=self.hierarchical_position,
-            embeddings_initializer=self.initializer,
-            name='Embedding-Position'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """GPT2的主体是基于Self-Attention的模块
-        顺序：LN --> Att  --> Add --> LN --> FFN --> Add
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-
-        # Self Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-        x = self.apply(
-            inputs=[x, x, x, attention_mask],
-            layer=MultiHeadAttention,
-            arguments={'a_bias': True},
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        return x
-
-    def apply_final_layers(self, inputs):
-        """剩余部分
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Output-Norm'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Output-Dropout'
-        )
-        x = super(GPT2, self).apply_final_layers(x)
-
-        return x
-
-    def variable_mapping(self):
-        """映射到TF版GPT2权重格式
-        """
-        mapping = super(GPT2, self).variable_mapping()
-        mapping = {
-            k: [i.replace('output/LayerNorm', 'input/LayerNorm') for i in v]
-            for k, v in mapping.items()
-        }
-        mapping['Output-Norm'] = [
-            'gpt/output/LayerNorm/beta',
-            'gpt/output/LayerNorm/gamma',
-        ]
-
-        return mapping
-
-
-class GPT2_ML(GPT):
-    """构建GPT2_ML模型
-    链接: https://github.com/imcaspar/gpt2-ml
-    注意：GPT2_ML虽然号称GPT2，但是它的结构其实更接近GPT，它自称GPT2的
-         原因大概是因为它开源的版本参数量达到了GPT2的15亿参数。
-    """
-    def get_inputs(self):
-        """GPT2_ML的输入是token_ids
-        """
-        x_in = self.apply(
-            layer=Input, shape=(self.sequence_length,), name='Input-Token'
-        )
-        return x_in
-
-    def apply_embeddings(self, inputs):
-        """GPT2_ML的embedding是token、position两者embedding之和
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=PositionEmbedding,
-            input_dim=self.max_position,
-            output_dim=self.embedding_size,
-            merge_mode='add',
-            hierarchical=self.hierarchical_position,
-            embeddings_initializer=self.initializer,
-            name='Embedding-Position'
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Embedding-Norm'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """GPT2_ML的主体是基于Self-Attention的模块
-        顺序：Att  --> LN --> FFN --> Add --> LN
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-
-        # Self Attention
-        xi, x, arguments = x, [x, x, x, attention_mask], {'a_bias': True}
-
-        x = self.apply(
-            inputs=x,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm-0' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            epsilon=1e-5,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm-1' % feed_forward_name
-        )
-
-        return x
-
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        variable = super(GPT2_ML, self).load_variable(checkpoint, name)
-        if name == 'newslm/embeddings/word_embed':
-            return self.load_embeddings(variable)
-        else:
-            return variable
-
-    def variable_mapping(self):
-        """映射到官方GPT2_ML权重格式
-        """
-        mapping = {
-            'Embedding-Token': ['newslm/embeddings/word_embed'],
-            'Embedding-Position': ['newslm/embeddings/pos_embed'],
-            'Embedding-Norm': [
-                'newslm/embeddings/LayerNorm_embed_norm/beta',
-                'newslm/embeddings/LayerNorm_embed_norm/gamma',
-            ],
-        }
-
-        for i in range(self.num_hidden_layers):
-            prefix = 'newslm/layer%02d/' % i
-            mapping.update({
-                'Transformer-%d-MultiHeadSelfAttention' % i: [
-                    prefix + 'query_layer/kernel',
-                    prefix + 'query_layer/bias',
-                    prefix + 'key_layer/kernel',
-                    prefix + 'key_layer/bias',
-                    prefix + 'value_layer/kernel',
-                    prefix + 'value_layer/bias',
-                    prefix + 'context_projection_layer/kernel',
-                    prefix + 'context_projection_layer/bias',
-                ],
-                'Transformer-%d-FeedForward-Norm-0' % i: [
-                    prefix + 'LayerNorm_mlp_ln0/beta',
-                    prefix + 'LayerNorm_mlp_ln0/gamma',
-                ],
-                'Transformer-%d-FeedForward' % i: [
-                    prefix + 'intermediate/kernel',
-                    prefix + 'intermediate/bias',
-                    prefix + 'output/kernel',
-                    prefix + 'output/bias',
-                ],
-                'Transformer-%d-FeedForward-Norm-1' % i: [
-                    prefix + 'LayerNorm_mlp_ln1/beta',
-                    prefix + 'LayerNorm_mlp_ln1/gamma',
-                ],
-            })
-
-        return mapping
-
-
-class T5_Base(Transformer):
-    """Google的T5模型（基类）
-    注意T5有两个版本，一开始放出来的版本称为t5.1.0，而后来放出了一个升级
-    版本称为t5.1.1，两者结构略有不同，包括后来放出来的多国语言版T5也采用
-    了t5.1.1的结构。
-    t5.1.0: https://github.com/google-research/text-to-text-transfer-transformer
-    t5.1.1: https://github.com/google-research/text-to-text-transfer-transformer/blob/master/released_checkpoints.md#t511
-    multilingual-t5: https://github.com/google-research/multilingual-t5
-    """
-    @insert_arguments(version='t5.1.0')
-    def __init__(self, **kwargs):
-        super(T5_Base, self).__init__(**kwargs)
-        self.p_bias = 't5_relative'
-    def load_variable(self, checkpoint, name):
-        """加载单个变量的函数
-        """
-        variable = super(T5_Base, self).load_variable(checkpoint, name)
-        if name == 'shared/embedding':
-            return self.load_embeddings(variable)
-        elif name == 'decoder/logits/kernel':
-            return self.load_embeddings(variable.T).T
-        elif 'relative_attention_bias' in name:
-            return variable.T
-        else:
-            return variable
-
-    def create_variable(self, name, value, dtype=None):
-        """在tensorflow中创建一个变量
-        """
-        if 'relative_attention_bias' in name:
-            value = value.T
-        return super(T5_Base, self).create_variable(name, value, dtype)
-
-    def variable_mapping(self):
-        """映射到官方T5权重格式
-        """
-        mapping = {
-            'Embedding-Token': ['shared/embedding'],
-            'Encoder-Embedding-Relative-Position': [
-                'encoder/block_000/layer_000/SelfAttention/relative_attention_bias'
-            ],
-            'Encoder-Output-Norm': ['encoder/final_layer_norm/scale'],
-            'Decoder-Embedding-Relative-Position': [
-                'decoder/block_000/layer_000/SelfAttention/relative_attention_bias',
-            ],
-            'Decoder-Output-Norm': ['decoder/final_layer_norm/scale'],
-        }
-
-        for i in range(self.num_hidden_layers):
-            # Encoder主体
-            prefix = 'encoder/block_%03d/' % i
-            mapping.update({
-                'Encoder-Transformer-%d-MultiHeadSelfAttention' % i: [
-                    prefix + 'layer_000/SelfAttention/q',
-                    prefix + 'layer_000/SelfAttention/k',
-                    prefix + 'layer_000/SelfAttention/v',
-                    prefix + 'layer_000/SelfAttention/o',
-                ],
-                'Encoder-Transformer-%d-MultiHeadSelfAttention-Norm' % i: [
-                    prefix + 'layer_000/layer_norm/scale',
-                ],
-                'Encoder-Transformer-%d-FeedForward' % i: [
-                    prefix + 'layer_001/DenseReluDense/wi/kernel',
-                    prefix + 'layer_001/DenseReluDense/wo/kernel',
-                ],
-                'Encoder-Transformer-%d-FeedForward-Norm' % i: [
-                    prefix + 'layer_001/layer_norm/scale',
-                ],
-            })
-            # Decoder主体
-            prefix = 'decoder/block_%03d/' % i
-            mapping.update({
-                'Decoder-Transformer-%d-MultiHeadSelfAttention' % i: [
-                    prefix + 'layer_000/SelfAttention/q',
-                    prefix + 'layer_000/SelfAttention/k',
-                    prefix + 'layer_000/SelfAttention/v',
-                    prefix + 'layer_000/SelfAttention/o',
-                ],
-                'Decoder-Transformer-%d-MultiHeadSelfAttention-Norm' % i: [
-                    prefix + 'layer_000/layer_norm/scale',
-                ],
-                'Decoder-Transformer-%d-MultiHeadCrossAttention' % i: [
-                    prefix + 'layer_001/EncDecAttention/q',
-                    prefix + 'layer_001/EncDecAttention/k',
-                    prefix + 'layer_001/EncDecAttention/v',
-                    prefix + 'layer_001/EncDecAttention/o',
-                ],
-                'Decoder-Transformer-%d-MultiHeadCrossAttention-Norm' % i: [
-                    prefix + 'layer_001/layer_norm/scale',
-                ],
-                'Decoder-Transformer-%d-FeedForward' % i: [
-                    prefix + 'layer_002/DenseReluDense/wi/kernel',
-                    prefix + 'layer_002/DenseReluDense/wo/kernel',
-                ],
-                'Decoder-Transformer-%d-FeedForward-Norm' % i: [
-                    prefix + 'layer_002/layer_norm/scale',
-                ],
-            })
-
-        if self.version.endswith('t5.1.1'):
-            mapping['Decoder-Output-LM'] = ['decoder/logits/kernel']
-            for i in range(self.num_hidden_layers):
-                for layer in [
-                    'Encoder-Transformer-%d-FeedForward' % i,
-                    'Decoder-Transformer-%d-FeedForward' % i
-                ]:
-                    mapping[layer] = [
-                        mapping[layer][0][:-7] + '_0' + mapping[layer][0][-7:],
-                        mapping[layer][0][:-7] + '_1' + mapping[layer][0][-7:],
-                        mapping[layer][1]
-                    ]
-            if self.version == 'mt5.1.1':
-                mapping['Encoder-Output-Norm'] = ['encoder/rms_norm/scale']
-                mapping['Decoder-Output-Norm'] = ['decoder/rms_norm/scale']
-                mapping = {
-                    k: [i.replace('layer_norm', 'rms_norm') for i in v]
-                    for k, v in mapping.items()
-                }
-
-        return mapping
-
-
-class T5_Encoder(T5_Base):
-    """Google的T5模型（Encoder）
-    """
-    def __init__(self,segment_size=0, **kwargs):
-        super(T5_Encoder, self).__init__(**kwargs)
-        self.segment_vocab_size=segment_size
-        
-
-    def get_inputs(self):
-        """T5的Encoder的输入只有token_ids
-        """
-        x_in = self.apply(
-            layer=Input,
-            shape=(self.sequence_length,),
-            name='Encoder-Input-Token'
-        )
-        if self.segment_vocab_size > 0:
-            s_in = self.apply(
-                layer=Input,
-                shape=(self.sequence_length,),
-                name='Segment-Input-Token'
-            )
-            return [x_in,s_in]
-        return x_in
-
-    def apply_embeddings(self, inputs):
-        """T5的embedding只有token embedding，
-        并把relative position embedding准备好，待attention使用。
-        """
-        if type(inputs)==list:
-            x,s = inputs[:]
-        else:
-            x = inputs
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        if self.segment_vocab_size > 0:
-            s = self.apply(
-                inputs=s,
-                layer=Embedding,
-                input_dim=self.segment_vocab_size,
-                output_dim=self.embedding_size,
-                embeddings_initializer='zeros',
-                name='Embedding-Segment'
-            )
-            x = self.apply(
-                inputs=[x, s], layer=Add, name='Embedding-Token-Segment'
-            )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Encoder-Embedding-Dropout'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Encoder-Embedding-Mapping'
-            )
-
-        return x
-
-    def apply_main_layers(self, inputs, index):
-        """T5的Encoder的主体是基于Self-Attention的模块
-        顺序：LN --> Att --> Add --> LN --> FFN --> Add
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        attention_name = 'Encoder-Transformer-%d-MultiHeadSelfAttention' % index
-        feed_forward_name = 'Encoder-Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias(x)
-
-        # Self Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % attention_name
-        )
-        x = self.apply(
-            inputs=[x, x, x, position_bias],
-            layer=MultiHeadAttention,
-            arguments={'p_bias': self.p_bias},
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            use_bias=False,
-            attention_scale=False,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            use_bias=False,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-
-        return x
-
-    def apply_final_layers(self, inputs):
-        """剩余部分
-        """
-        x = inputs
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Encoder-Output-Norm'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Encoder-Output-Dropout'
-        )
-
-        return x
-
-    def compute_position_bias(self, inputs=None):
-        """T5相对位置编码
-        """
-        if self.position_bias is None:
-
-            x = inputs
-            p = self.apply(
-                inputs=[x, x],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=True,
-                embeddings_initializer=self.initializer,
-                name='Encoder-Embedding-Relative-Position'
-            )
-            self.position_bias = p
-
-        return self.position_bias
-    
-
-class T5_Decoder(LM_Mask, T5_Base):
-    """Google的T5模型（Decoder）
-    """
-    def __init__(self, with_lm=True, cross_position_bias=True,logit_scale=True, decoder_sequence_length=None,**kwargs):
-        super(T5_Decoder, self).__init__(**kwargs)
-        self.with_lm = with_lm
-        self.cross_position_bias = cross_position_bias
-        self.logit_scale=logit_scale
-        self.is_seq2seq = True
-        self.decoder_sequence_length=decoder_sequence_length
-    def get_inputs(self):
-        """T5的Decoder的输入为context序列和token_ids
-        """
-        c_in = self.apply(
-            layer=Input,
-            shape=(self.sequence_length, self.hidden_size),
-            name='Input-Context'
-        )
-        x_in = self.apply(
-            layer=Input,
-            shape=(self.decoder_sequence_length,),
-            name='Decoder-Input-Token'
-        )
-        return [c_in, x_in]
-
-    def apply_embeddings(self, inputs):
-        """T5的embedding只有token embedding，
-        并把relative position embedding准备好，待attention使用。
-        """
-        c, x = inputs
-
-        x = self.apply(
-            inputs=x,
-            layer=Embedding,
-            input_dim=self.vocab_size,
-            output_dim=self.embedding_size,
-            embeddings_initializer=self.initializer,
-            mask_zero=True,
-            name='Embedding-Token'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Decoder-Embedding-Dropout'
-        )
-        if self.embedding_size != self.hidden_size:
-            x = self.apply(
-                inputs=x,
-                layer=Dense,
-                units=self.hidden_size,
-                kernel_initializer=self.initializer,
-                name='Decoder-Embedding-Mapping'
-            )
-
-        return [c, x]
-
-    def apply_main_layers(self, inputs, index):
-        """T5的Decoder主体是基于Self-Attention、Cross-Attention的模块
-        顺序：LN --> Att1 --> Add --> LN --> Att2 --> Add -->  LN --> FFN --> Add
-        """
-        c, x = inputs
-        z = self.layer_norm_conds[0]
-
-        self_attention_name = 'Decoder-Transformer-%d-MultiHeadSelfAttention' % index
-        cross_attention_name = 'Decoder-Transformer-%d-MultiHeadCrossAttention' % index
-        feed_forward_name = 'Decoder-Transformer-%d-FeedForward' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias([x, c])
-
-        # Self Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % self_attention_name
-        )
-        p = position_bias
-        if self.p_bias=='t5_relative':
-            p = position_bias[0]
-        x = self.apply(
-            inputs=[x, x, x, attention_mask,p ],
-            layer=MultiHeadAttention,
-            arguments={
-                'a_bias': True,
-                'p_bias': self.p_bias
-            },
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            use_bias=False,
-            attention_scale=False,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=self_attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % self_attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % self_attention_name
-        )
-
-        # Cross Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % cross_attention_name
-        )
-        if self.cross_position_bias:
-            inputs = [x, c, c, position_bias[1]]
-            arguments = {'a_bias': None, 'p_bias': self.p_bias}
-        else:
-            inputs = [x, c, c]
-            arguments = {'a_bias': None, 'p_bias': None}
-        x = self.apply(
-            inputs=inputs,
-            layer=MultiHeadAttention,
-            arguments=arguments,
-            heads=self.num_attention_heads,
-            head_size=self.attention_head_size,
-            out_dim=self.hidden_size,
-            key_size=self.attention_key_size,
-            use_bias=False,
-            attention_scale=False,
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=cross_attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % cross_attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % cross_attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='%s-Norm' % feed_forward_name
-        )
-        x = self.apply_ffn_layer(x,feed_forward_name)
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % feed_forward_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-
-        return [c, x]
-    def apply_ffn_layer(self,x,feed_forward_name):
-        return self.apply(
-            inputs=x,
-            layer=FeedForward,
-            units=self.intermediate_size,
-            activation=self.hidden_act,
-            use_bias=False,
-            kernel_initializer=self.initializer,
-            name=feed_forward_name
-        )
-    def apply_final_layers(self, inputs):
-        """剩余部分
-        """
-        c, x = inputs
-        z = self.layer_norm_conds[0]
-
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            layer=LayerNormalization,
-            zero_mean=False,
-            offset=False,
-            epsilon=1e-6,
-            conditional=(z is not None),
-            hidden_units=self.layer_norm_conds[1],
-            hidden_activation=self.layer_norm_conds[2],
-            hidden_initializer=self.initializer,
-            name='Decoder-Output-Norm'
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='Decoder-Output-Dropout'
-        )
-        if self.logit_scale:
-            x = self.apply(
-                inputs=x,
-                layer=ScaleOffset,
-                scale=self.hidden_size**(-0.5),
-                offset=False,
-                name='Decoder-Output-Scale'
-            )
-
-        if self.with_lm:
-            # 预测token概率部分
-            if self.embedding_size != self.hidden_size:
-                x = self.apply(
-                    inputs=x,
-                    layer=Dense,
-                    units=self.embedding_size,
-                    kernel_initializer=self.initializer,
-                    name='Decoder-Output-Mapping'
-                )
-            lm_activation = 'softmax' if self.with_lm is True else self.with_lm
-            if self.version == 't5.1.0':
-                x = self.apply(
-                    inputs=x,
-                    layer=Embedding,
-                    arguments={'mode': 'dense'},
-                    name='Embedding-Token'
-                )
-                x = self.apply(
-                    inputs=x,
-                    layer=Activation,
-                    activation=lm_activation,
-                    name='Decoder-Output-LM-Activation'
-                )
-            else:
-                x = self.apply(
-                    inputs=x,
-                    layer=Dense,
-                    units=self.vocab_size,
-                    activation=lm_activation,
-                    use_bias=False,
-                    kernel_initializer=self.initializer,
-                    name='Decoder-Output-LM'
-                )
-
-        return x
-
-    def compute_attention_bias(self, inputs=None):
-        """修改LM Mask的序列长度（从 self.inputs[0] 改为 self.inputs[1] ）
-        """
-        old_inputs = self.inputs[:]
-        self.inputs = [old_inputs[1]]
-        mask = super(T5_Decoder, self).compute_attention_bias(inputs)
-        self.inputs = old_inputs
-        return mask
-
-    def compute_position_bias(self, inputs=None):
-        """T5相对位置编码
-        """
-        if self.position_bias is None:
-
-            x, c = inputs
-            p1 = self.apply(
-                inputs=[x, x],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            p2 = self.apply(
-                inputs=[x, c],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            self.position_bias = (p1, p2)
-
-        return self.position_bias
-    def get_cache_inputs(self,lengths:list):
-        """Misaka的Decoder的输入为context序列和token_ids
-        """
-        c_in = self.apply(
-            layer=Input,
-            shape=(lengths[0], self.hidden_size),
-            name='Input-Context-cache-'+str(lengths[1])
-        )
-        x_in = self.apply(
-            layer=Input,
-            shape=[lengths[1]],
-            name='Decoder-Input-Token-cache-'+str(lengths[1])
-        )
-        return [c_in, x_in] 
-    def compute_attention_bias(self, inputs=None):
-        """修改LM Mask的序列长度（从 self.inputs[0] 改为 self.inputs[1] ）
-        """
-        old_inputs = self.inputs[:]
-        self.inputs = [old_inputs[1]]
-        mask = super(T5_Decoder, self).compute_attention_bias(inputs)
-        self.inputs = old_inputs
-        return mask
-
-    def compute_position_bias(self, inputs=None):
-        """T5相对位置编码
-        """
-        if self.position_bias is None:
-
-            x, c = inputs
-            p1 = self.apply(
-                inputs=[x, x],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            p2 = self.apply(
-                inputs=[x, c],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            self.position_bias = (p1, p2)
-
-        return self.position_bias
-    def compute_cache_position_bias(self, inputs=None,self_cache_update_index=None,index=None):
-        """T5相对位置编码
-        """
-        if self.cache_position_bias is None:
-
-            c,x = inputs
-            p1 = self.apply(
-                inputs=[x, x],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            p2 = self.apply(
-                inputs=[x, c],
-                layer=RelativePositionEmbeddingT5,
-                input_dim=32,
-                output_dim=self.num_attention_heads,
-                bidirectional=False,
-                embeddings_initializer=self.initializer,
-                name='Decoder-Embedding-Relative-Position'
-            )
-            self.cache_position_bias = (p1, p2)
-        if inputs!=None:
-            return None
-        p1,p2=self.cache_position_bias
-
-
-        p1 = self.apply(
-            inputs=p1,
-            layer=TakeLayer,
-            arguments={'index': self_cache_update_index},
-            name='TakeLayer'
-        )
-        
-        p2 = self.apply(
-            inputs=p2,
-            layer=TakeLayer,
-            arguments={'index': self_cache_update_index},
-            name='TakeLayer'
-        )
-        self.length_cache_position_bias = [p1,p2]
-        
-        return self.length_cache_position_bias
-
-    def apply_main_cache_layers(self, inputs, index,self_cache_update_index,
-                                cross_cache_update_index=None,
-                                attention_mask=None,position_bias=None,
-            
-                                ):
-        """T5的Decoder主体是基于Self-Attention、Cross-Attention的模块
-        顺序：LN --> Att1 --> Add --> LN --> Att2 --> Add -->  LN --> FFN --> Add
-        """
-        c, x ,caches = inputs
-        z = self.layer_norm_conds[0]
-
-        self_attention_name = 'Decoder-Transformer-%d-MultiHeadSelfAttention' % index
-        cross_attention_name = 'Decoder-Transformer-%d-MultiHeadCrossAttention' % index
-        feed_forward_name = 'Decoder-Transformer-%d-FeedForward' % index
-
-        
-        # Self Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % self_attention_name
-        )
-        arguments={
-                'a_bias': True,
-                'p_bias': self.p_bias,
-                'cache_update_index':True,
-                'use_cache':True,
-            }
-        p = position_bias
-        if self.p_bias == 't5_relative':
-            p = position_bias[0]
-            inputs = [x, x, x, attention_mask,caches[0],self_cache_update_index,p]
-        else:
-            inputs = [x, x, x, attention_mask,p,caches[0],self_cache_update_index]
-        x,cache_self = self.apply(
-            inputs=inputs,
-            arguments=arguments,
-            name=self_attention_name
-        )
-        caches[0]=cache_self
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % self_attention_name
-        )
-
-        # Cross Attention
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % cross_attention_name
-        )
-        if self.cross_position_bias:
-            inputs = [x, c, c, position_bias[1]]
-            arguments = {'a_bias': None, 'p_bias': self.p_bias}
-        else:
-            inputs = [x, c, c]
-            arguments = {'a_bias': None, 'p_bias': None}
-        arguments['use_cache']=True
-        
-        inputs.insert(3,caches[1])
-        if cross_cache_update_index is None:
-            arguments['cache_update_index']=False
-        else:
-            arguments['cache_update_index']=True
-            inputs.insert(4,cross_cache_update_index)
-
-        x ,cross_cache = self.apply(
-                inputs=inputs,
-                arguments=arguments,
-                name=cross_attention_name
-            )
-        caches[1]=cross_cache
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % cross_attention_name
-        )
-
-        # Feed Forward
-        xi = x
-        x = self.apply(
-            inputs=self.simplify([x, z]),
-            name='%s-Norm' % feed_forward_name
-        )
-        x = self.apply_ffn_layer(x,feed_forward_name)
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % feed_forward_name
-        )
-
-        return [c, x ,caches]
-class T5(T5_Base):
-    """Google的T5模型（Encoder-Decoder）
-    """
-    def __init__(self, **kwargs):
-        super(T5, self).__init__(**kwargs)
-        kwargs['layers'] = self.layers
-        e_name, d_name = 'Encoder', 'Decoder'
-        if 'name' in kwargs:
-            e_name = '%s_%s' % (kwargs['name'], e_name)
-            d_name = '%s_%s' % (kwargs['name'], d_name)
-            del kwargs['name']  # 防止重复传参
-        self._encoder = T5_Encoder(name=e_name, **kwargs)
-        self._decoder = T5_Decoder(name=d_name, **kwargs)
-
-    def build(self, **kwargs):
-        """同时构建Encoder和Decoder
-        """
-        self._encoder.build(**kwargs)
-        self._decoder.build(**kwargs)
-        self._decoder.position_bias = None  # 下面call时将重新初始化
-        self.encoder = self._encoder.model
-        self.decoder = self._decoder.model
-        self.inputs = self.encoder.inputs + self.decoder.inputs[1:]
-        self.outputs = self._decoder.call(
-            self.encoder.outputs + self.decoder.inputs[1:]
-        )
-        self.model = Model(self.inputs, self.outputs)
-    def build_cache_model(self,input_lengths:list,end_token,search_mode='greedy',k=1,progress_print=False,index_bias=0):
-        self.cache_decoder = self._decoder.build_cache_model(input_lengths,end_token,
-                                                    search_mode,k,
-                                                    progress_print,
-                                                    index_bias)
-        y = self.cache_decoder([self.encoder.output,self.cache_decoder.inputs[1]])
-        self.cache_t5 = keras.Model(self.encoder.inputs[:]+self.cache_decoder.inputs[1:],y)
-
-        return self.cache_t5
-class MisakaT5(T5):
-    """Google的T5模型（Encoder-Decoder）
-    """
-    def __init__(self, **kwargs):
-        super(T5, self).__init__(**kwargs)
-        kwargs['layers'] = self.layers
-        e_name, d_name = 'Encoder', 'Decoder'
-        if 'name' in kwargs:
-            e_name = '%s_%s' % (kwargs['name'], e_name)
-            d_name = '%s_%s' % (kwargs['name'], d_name)
-            del kwargs['name']  # 防止重复传参
-        self._encoder = MisakaT5_Encoder(name=e_name, **kwargs)
-        self._decoder = MisakaT5_Decoder(name=d_name, **kwargs)
+from bert4keras3.transformers import *
+from bert4keras3.Models.Berts import *
+from bert4keras3.Models.Alberts import *
+from bert4keras3.Models.Roformers import *
+from bert4keras3.Models.GPTs import *
+from bert4keras3.Models.T5models import *
+from bert4keras3.Models.GPTs import *
+from bert4keras3.Models.GAUs import *
+from bert4keras3.Models.LLamas import *
 def extend_with_language_model(BaseModel):
     """添加下三角的Attention Mask（语言模型用）
     """
     class LanguageModel(LM_Mask, BaseModel):
         """带下三角Attention Mask的派生模型
         """
         def __init__(self, *args, **kwargs):
@@ -3267,162 +35,15 @@
         def __init__(self, *args, **kwargs):
             super(UnifiedLanguageModel, self).__init__(*args, **kwargs)
             self.with_mlm = self.with_mlm or True
 
     return UnifiedLanguageModel
 
 
-class GAU_alpha(RoFormerV2):
-    """GAU-α
-    改动：基本模块换成GAU
-    链接：https://kexue.fm/archives/9052
-    """
-    def initializer(self, shape, dtype=None, order=3, gain=1.0):
-        return super(GAU_alpha, self).initializer(shape, dtype, order, gain)
-
-    def apply_main_layers(self, inputs, index):
-        """GAU-α 的主体是基于Gated Attention Unit的模块
-        顺序：GAU  --> Add --> LN
-        """
-        x = inputs
-
-        attention_name = 'Transformer-%d-GatedAttentionUnit' % index
-        attention_mask = self.compute_attention_bias(index)
-        position_bias = self.compute_position_bias(x)
-
-        # Self Attention
-        xi = x
-        x = [x, position_bias]
-        arguments = {'a_bias': None, 'p_bias': 'rotary'}
-        if attention_mask is not None:
-            arguments['a_bias'] = True
-            x.insert(1, attention_mask)
-        x = self.apply(
-            inputs=x,
-            layer=GatedAttentionUnit,
-            arguments=arguments,
-            units=self.intermediate_size,
-            key_size=self.attention_key_size,
-            activation=self.hidden_act,
-            use_bias=False,
-            normalization='softmax_plus',
-            attention_dropout=self.attention_dropout_rate,
-            kernel_initializer=self.initializer,
-            name=attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=Dropout,
-            rate=self.dropout_rate,
-            name='%s-Dropout' % attention_name
-        )
-        x = self.apply(
-            inputs=[xi, x], layer=Add, name='%s-Add' % attention_name
-        )
-        x = self.apply(
-            inputs=x,
-            layer=LayerNormalization,
-            zero_mean=False,
-            scale=False,
-            offset=False,
-            name='%s-Norm' % attention_name
-        )
-
-        return x
-
-    def variable_mapping(self):
-        """重新定义权重映射
-        """
-        mapping = {
-            'Embedding-Token': ['bert/embeddings/word_embeddings'],
-            'Embedding-Segment': ['bert/embeddings/token_type_embeddings'],
-        }
-
-        for i in range(self.num_hidden_layers):
-            prefix = 'GAU_alpha/encoder/layer_%d/' % i
-            
-            mapping['Transformer-%d-GatedAttentionUnit' % i] = [
-                prefix + 'gau/i_dense/kernel',
-                # prefix + 'gau/i_dense/bias',
-                # prefix + 'gau/q_scaleoffset/beta',
-                prefix + 'gau/q_scaleoffset/gamma',
-                # prefix + 'gau/k_scaleoffset/beta',
-                prefix + 'gau/k_scaleoffset/gamma',
-                prefix + 'gau/o_dense/kernel',
-                # prefix + 'gau/o_dense/bias',
-            ]
-
-        return mapping
-
-
-class MisakaT5_Encoder(T5_Encoder):
-    def __init__(self, **kwargs):
-        super( MisakaT5_Encoder, self).__init__(**kwargs)
-        self.p_bias = 'rotary'
-    def compute_position_bias(self, inputs=None):
-        """Sinusoidal位置编码（直接返回）
-        """
-        if self.position_bias is None:
-
-            if self.custom_position_ids:
-                x = [inputs, self.inputs[2]]
-            else:
-                x = inputs
-
-            self.position_bias = self.apply(
-                inputs=x,
-                layer=SinusoidalPositionEmbedding,
-                output_dim=self.attention_key_size,
-                merge_mode='zero',
-                custom_position_ids=self.custom_position_ids,
-                name='Embedding-Rotary-Position'
-            )
-
-        return self.position_bias
-class MisakaT5_Decoder(T5_Decoder):
-    def __init__(self, **kwargs):
-        super( MisakaT5_Decoder, self).__init__(**kwargs)
-        self.p_bias = 'rotary'
-    def compute_cache_position_bias(self, inputs=None,self_cache_update_index=None,index=None):
-        if self.cache_position_bias is None:
-
-            self.cache_position_bias =self.apply(
-                inputs=inputs[1],
-                name='Embedding-Rotary-Position'
-            )
-        if inputs!=None:
-            return None
-        self.length_cache_position_bias = self.apply(
-            inputs=self.cache_position_bias,
-            layer=TakeLayer,
-            axis=1,
-            arguments={'index': self_cache_update_index},
-            name='TakeLayer'
-        )
-        
-        return self.length_cache_position_bias
-    def compute_position_bias(self, inputs=None):
-        """Sinusoidal位置编码（直接返回）
-        """
-        
-        if self.position_bias is None:
-
-            x, c = inputs[:]
-           
-            self.position_bias = self.apply(
-                inputs=x,
-                layer=SinusoidalPositionEmbedding,
-                output_dim=self.attention_key_size,
-                merge_mode='zero',
-                custom_position_ids=self.custom_position_ids,
-                name='Embedding-Rotary-Position'
-            )
 
-        return self.position_bias
-        
 
 def build_transformer_model(
     config_path=None,
     checkpoint_path=None,
     model='bert',
     application='encoder',
     return_keras_model=True,
@@ -3467,14 +88,18 @@
         't5.1.0_decoder': T5_Decoder,
         't5.1.1': T5,
         't5.1.1_encoder': T5_Encoder,
         't5.1.1_decoder': T5_Decoder,
         'mt5.1.1': T5,
         'mt5.1.1_encoder': T5_Encoder,
         'mt5.1.1_decoder': T5_Decoder,
+        'gemma':Gemma,
+        'llama':Llama, 
+        'qwen':Llama, 
+        'yi':Llama, 
         'misakat5':MisakaT5,
     }
 
     if is_string(model):
         model = model.lower()
         MODEL = models[model]
         if model.startswith('t5.1.1'):
@@ -3504,24 +129,24 @@
         for modelin in transformer.model.inputs: 
             shape=keras.ops.shape(modelin)
             shape=[1 if t==None else t for t in shape]
             try:
                 shape[0] = len(keras.distribution.list_devices())
             except:
                 pass
-            inputs.append(np.zeros(shape,modelin.dtype))
+            inputs.append(np.ones(shape,modelin.dtype))
         transformer.model.predict(inputs,verbose=3)
         if keras_weights_path is not None:
             transformer.model.load_weights(keras_weights_path, skip_mismatch=True)
         if lora_model:
             
             def enable_lora(t):
                 if isinstance(t,keras.layers.Embedding) :
                     t.enable_lora(kwargs['attention_head_size']*2)
-                elif isinstance(t,keas.layers.Dense):
+                elif isinstance(t,keras.layers.Dense):
                     t.enable_lora(kwargs['attention_head_size'])
             for layer in transformer.model.layers:
                 layer.trainable=False
                 enable_lora(layer)
                 for kid in dir (layer):
                     t = getattr(layer,kid)
                     enable_lora(t)
```

## Comparing `bert4keras3-1.2.9.dist-info/LICENSE` & `bert4keras3-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bert4keras3-1.2.9.dist-info/RECORD` & `bert4keras3-1.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-bert4keras3/__init__.py,sha256=CMb8S8X82Zw-9GhxgUom0I8qs7veKePBxPqa7nStNpk,150
-bert4keras3/backend.py,sha256=6Z7XUI2vjPtrddejf0y2rCKQftucxxCf74jjwGPs1l0,20229
-bert4keras3/layers.py,sha256=PvlMvpDjIZaIgNSJ5gfzyTgoDyK5GhhonPqJhrb16d4,52459
-bert4keras3/models.py,sha256=TOCiCb3GgAd33dsW2rRGRBxmlhBGoUKWDfF7zkkRlec,124407
+bert4keras3/__init__.py,sha256=cQCKzarpKN-VHmivGnetot0AdqJIjBwTz5CWB38gagc,148
+bert4keras3/backend.py,sha256=1ywO73bYuMXA5CpAkRNcxpOExa7WCKrj9ryooJxCzP0,23204
+bert4keras3/layers.py,sha256=wSLeVRzTvWoonglKhQl8sQ2HbmlZBJis7KNTOiiPwf8,11442
+bert4keras3/models.py,sha256=o7DHSr3Dvj7IIa5oVBqyO92fIm2oLU-pPoo5YsSlNaU,5211
 bert4keras3/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
 bert4keras3/snippets.py,sha256=YwdYRvrewhM6g8ax9_Ath0HsJATzuyZksL5Dow9l65A,27955
 bert4keras3/tokenizers.py,sha256=PCxtC4L9tF2w-GUDujdPK8Z5WlnbaL8mYhRfHn1S_Qg,15509
-bert4keras3-1.2.9.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-bert4keras3-1.2.9.dist-info/METADATA,sha256=A3f411Oo1Go23bwchoY85RTIWqCx_YlhSTXW-Vo3t7Y,221
-bert4keras3-1.2.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-bert4keras3-1.2.9.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
-bert4keras3-1.2.9.dist-info/RECORD,,
+bert4keras3/transformers.py,sha256=QC9926N2XJokR5oS9ZdDSaxZwwA15MVdpLrPxcUArxk,28534
+bert4keras3-1.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+bert4keras3-1.3.dist-info/METADATA,sha256=5p3NMnrqU568-TO88A-cBR5kwse9zeq_dGkqIplgTcU,219
+bert4keras3-1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+bert4keras3-1.3.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
+bert4keras3-1.3.dist-info/RECORD,,
```

