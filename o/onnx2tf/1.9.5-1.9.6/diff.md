# Comparing `tmp/onnx2tf-1.9.5.tar.gz` & `tmp/onnx2tf-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2tf-1.9.5.tar", last modified: Sun Apr 16 05:11:48 2023, max compression
+gzip compressed data, was "onnx2tf-1.9.6.tar", last modified: Sun Apr 16 08:51:18 2023, max compression
```

## Comparing `onnx2tf-1.9.5.tar` & `onnx2tf-1.9.6.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/LICENSE_onnx-tensorflow
--rw-r--r--   0 runner    (1001) docker     (123)   104976 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   104434 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.343809 onnx2tf-1.9.5/onnx2tf/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/onnx2tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/onnx2tf/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Abs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Acos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Acosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/And.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ArgMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ArgMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Asin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Asinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Atan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Atanh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/AveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/BatchNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Bernoulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/BitShift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Celu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ConcatFromSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ConstantOfShape.py
--rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ConvTranspose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Cos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Cosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/CumSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/DepthToSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/DequantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Det.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Div.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/DynamicQuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Einsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Elu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Equal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Erf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/EyeLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/FusedConv.py
--rw-r--r--   0 runner    (1001) docker     (123)    30610 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GRU.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GatherElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GatherND.py
--rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Gemm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GlobalAveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GlobalLpPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GlobalMaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Greater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GreaterOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/GridSample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/HardSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/HardSwish.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Hardmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/If.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/InstanceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/IsInf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/IsNaN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LRN.py
--rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LayerNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Less.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LessOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LogSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/LpNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/MatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/MatMulInteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Max.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/MaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/MaxUnpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/MeanVarianceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Min.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Mul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Multinomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Neg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/NonMaxSuppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/NonZero.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Not.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/OneHot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Or.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/PRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Pow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearAdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearConcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearLeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearMatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QLinearSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/QuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RNN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RandomNormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RandomNormalLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RandomUniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RandomUniformLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceL1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceL2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceLogSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceLogSumExp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceMean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceProd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReduceSumSquare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Relu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ReverseSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/RoiAlign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Round.py
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ScaleAndTranslate.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ScatterElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ScatterND.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Selu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceConstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceEmpty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceErase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceInsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SequenceLength.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Shrink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Size.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Softplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Softsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SpaceToDepth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/SplitToSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Tan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/ThresholdedRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/TopK.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Trilu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Where.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/Xor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/_Loop.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/onnx2tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)   199977 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/utils/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/onnx2tf/utils/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.343809 onnx2tf-1.9.5/onnx2tf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   104976 2023-04-16 05:11:48.000000 onnx2tf-1.9.5/onnx2tf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-16 05:11:48.000000 onnx2tf-1.9.5/onnx2tf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:11:48.000000 onnx2tf-1.9.5/onnx2tf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 05:11:48.000000 onnx2tf-1.9.5/onnx2tf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 05:11:48.000000 onnx2tf-1.9.5/onnx2tf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:48.367809 onnx2tf-1.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-16 05:11:40.000000 onnx2tf-1.9.5/tests/test_model_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/LICENSE_onnx-tensorflow
+-rw-r--r--   0 runner    (1001) docker     (123)   104992 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   104450 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.131524 onnx2tf-1.9.6/onnx2tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/onnx2tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/onnx2tf/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Acos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Acosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/And.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ArgMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ArgMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Asin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Asinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Atan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Atanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/AveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/BatchNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/BitShift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Celu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ConcatFromSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ConstantOfShape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ConvTranspose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Cosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/CumSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/DepthToSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/DequantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Det.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Div.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/DynamicQuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Elu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/EyeLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/FusedConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30610 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GRU.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GatherElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GatherND.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Gemm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GlobalAveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GlobalLpPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GlobalMaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Greater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GreaterOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/GridSample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/HardSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/HardSwish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Hardmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/InstanceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/IsInf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/IsNaN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LRN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LayerNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Less.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LessOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LogSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/LpNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/MatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/MatMulInteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Max.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/MaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/MaxUnpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/MeanVarianceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/NonMaxSuppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/NonZero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/OneHot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Or.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/PRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Pow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearAdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearConcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearLeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearMatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QLinearSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/QuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RandomNormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RandomNormalLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RandomUniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RandomUniformLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceL1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceL2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceLogSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceLogSumExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceMean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceProd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReduceSumSquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ReverseSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/RoiAlign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Round.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ScaleAndTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ScatterElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ScatterND.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Selu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceConstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceEmpty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceErase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceInsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SequenceLength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Shrink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Softsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SpaceToDepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/SplitToSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Tan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/ThresholdedRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/TopK.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Trilu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/Xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/_Loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/onnx2tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199977 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/utils/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/onnx2tf/utils/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.135524 onnx2tf-1.9.6/onnx2tf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   104992 2023-04-16 08:51:18.000000 onnx2tf-1.9.6/onnx2tf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-16 08:51:18.000000 onnx2tf-1.9.6/onnx2tf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:51:18.000000 onnx2tf-1.9.6/onnx2tf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 08:51:18.000000 onnx2tf-1.9.6/onnx2tf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:51:18.000000 onnx2tf-1.9.6/onnx2tf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:51:18.155523 onnx2tf-1.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-16 08:51:09.000000 onnx2tf-1.9.6/tests/test_model_convert.py
```

### Comparing `onnx2tf-1.9.5/LICENSE` & `onnx2tf-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/LICENSE_onnx-tensorflow` & `onnx2tf-1.9.6/LICENSE_onnx-tensorflow`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/PKG-INFO` & `onnx2tf-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2tf
-Version: 1.9.5
+Version: 1.9.6
 Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
 Home-page: https://github.com/PINTO0309/onnx2tf
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -252,23 +252,23 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.5
+  ghcr.io/pinto0309/onnx2tf:1.9.6
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
-  && pip install -U onnxsim \
+  && pip install -U onnxsim==0.4.17 \
   && pip install -U simple_onnx_processing_tools \
   && pip install -U onnx2tf \
   && pip install -U h5py==3.7.0
 
   or
 
   $ pip install -e .
@@ -295,15 +295,15 @@
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 2
   !python3.9 -m pip install tensorflow==2.12.0 \
     && python3.9 -m pip install -U onnx \
     && python3.9 -m pip install -U nvidia-pyindex \
     && python3.9 -m pip install -U onnx-graphsurgeon \
     && python3.9 -m pip install -U onnxruntime==1.13.1 \
-    && python3.9 -m pip install -U onnxsim \
+    && python3.9 -m pip install -U onnxsim==0.4.17 \
     && python3.9 -m pip install -U simple_onnx_processing_tools \
     && python3.9 -m pip install -U onnx2tf \
     && python3.9 -m pip install -U protobuf==3.20.3 \
     && python3.9 -m pip install -U h5py==3.7.0
   ```
 
 ### 2. Run test
```

### Comparing `onnx2tf-1.9.5/README.md` & `onnx2tf-1.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -237,23 +237,23 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.5
+  ghcr.io/pinto0309/onnx2tf:1.9.6
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
-  && pip install -U onnxsim \
+  && pip install -U onnxsim==0.4.17 \
   && pip install -U simple_onnx_processing_tools \
   && pip install -U onnx2tf \
   && pip install -U h5py==3.7.0
 
   or
 
   $ pip install -e .
@@ -280,15 +280,15 @@
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 2
   !python3.9 -m pip install tensorflow==2.12.0 \
     && python3.9 -m pip install -U onnx \
     && python3.9 -m pip install -U nvidia-pyindex \
     && python3.9 -m pip install -U onnx-graphsurgeon \
     && python3.9 -m pip install -U onnxruntime==1.13.1 \
-    && python3.9 -m pip install -U onnxsim \
+    && python3.9 -m pip install -U onnxsim==0.4.17 \
     && python3.9 -m pip install -U simple_onnx_processing_tools \
     && python3.9 -m pip install -U onnx2tf \
     && python3.9 -m pip install -U protobuf==3.20.3 \
     && python3.9 -m pip install -U h5py==3.7.0
   ```
 
 ### 2. Run test
```

### Comparing `onnx2tf-1.9.5/onnx2tf/onnx2tf.py` & `onnx2tf-1.9.6/onnx2tf/onnx2tf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Abs.py` & `onnx2tf-1.9.6/onnx2tf/ops/Abs.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Acos.py` & `onnx2tf-1.9.6/onnx2tf/ops/Acos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Acosh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Acosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Add.py` & `onnx2tf-1.9.6/onnx2tf/ops/Add.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/And.py` & `onnx2tf-1.9.6/onnx2tf/ops/And.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ArgMax.py` & `onnx2tf-1.9.6/onnx2tf/ops/ArgMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ArgMin.py` & `onnx2tf-1.9.6/onnx2tf/ops/ArgMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Asin.py` & `onnx2tf-1.9.6/onnx2tf/ops/Asin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Asinh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Asinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Atan.py` & `onnx2tf-1.9.6/onnx2tf/ops/Atan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Atanh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Atanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/AveragePool.py` & `onnx2tf-1.9.6/onnx2tf/ops/AveragePool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/BatchNormalization.py` & `onnx2tf-1.9.6/onnx2tf/ops/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Bernoulli.py` & `onnx2tf-1.9.6/onnx2tf/ops/Bernoulli.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/BitShift.py` & `onnx2tf-1.9.6/onnx2tf/ops/BitShift.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Cast.py` & `onnx2tf-1.9.6/onnx2tf/ops/Cast.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Ceil.py` & `onnx2tf-1.9.6/onnx2tf/ops/Ceil.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Celu.py` & `onnx2tf-1.9.6/onnx2tf/ops/Celu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Clip.py` & `onnx2tf-1.9.6/onnx2tf/ops/Clip.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Compress.py` & `onnx2tf-1.9.6/onnx2tf/ops/Compress.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Concat.py` & `onnx2tf-1.9.6/onnx2tf/ops/Concat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ConcatFromSequence.py` & `onnx2tf-1.9.6/onnx2tf/ops/ConcatFromSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Constant.py` & `onnx2tf-1.9.6/onnx2tf/ops/Constant.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ConstantOfShape.py` & `onnx2tf-1.9.6/onnx2tf/ops/ConstantOfShape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Conv.py` & `onnx2tf-1.9.6/onnx2tf/ops/Conv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ConvTranspose.py` & `onnx2tf-1.9.6/onnx2tf/ops/ConvTranspose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Cos.py` & `onnx2tf-1.9.6/onnx2tf/ops/Cos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Cosh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Cosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/CumSum.py` & `onnx2tf-1.9.6/onnx2tf/ops/CumSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/DepthToSpace.py` & `onnx2tf-1.9.6/onnx2tf/ops/DepthToSpace.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/DequantizeLinear.py` & `onnx2tf-1.9.6/onnx2tf/ops/DequantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Det.py` & `onnx2tf-1.9.6/onnx2tf/ops/Det.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Div.py` & `onnx2tf-1.9.6/onnx2tf/ops/Div.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Dropout.py` & `onnx2tf-1.9.6/onnx2tf/ops/Dropout.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/DynamicQuantizeLinear.py` & `onnx2tf-1.9.6/onnx2tf/ops/DynamicQuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Einsum.py` & `onnx2tf-1.9.6/onnx2tf/ops/Einsum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Elu.py` & `onnx2tf-1.9.6/onnx2tf/ops/Elu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Equal.py` & `onnx2tf-1.9.6/onnx2tf/ops/Equal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Erf.py` & `onnx2tf-1.9.6/onnx2tf/ops/Erf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Exp.py` & `onnx2tf-1.9.6/onnx2tf/ops/Exp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Expand.py` & `onnx2tf-1.9.6/onnx2tf/ops/Expand.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/EyeLike.py` & `onnx2tf-1.9.6/onnx2tf/ops/EyeLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Flatten.py` & `onnx2tf-1.9.6/onnx2tf/ops/Flatten.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Floor.py` & `onnx2tf-1.9.6/onnx2tf/ops/Floor.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/FusedConv.py` & `onnx2tf-1.9.6/onnx2tf/ops/FusedConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GRU.py` & `onnx2tf-1.9.6/onnx2tf/ops/GRU.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Gather.py` & `onnx2tf-1.9.6/onnx2tf/ops/Gather.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GatherElements.py` & `onnx2tf-1.9.6/onnx2tf/ops/GatherElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GatherND.py` & `onnx2tf-1.9.6/onnx2tf/ops/GatherND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Gemm.py` & `onnx2tf-1.9.6/onnx2tf/ops/Gemm.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GlobalAveragePool.py` & `onnx2tf-1.9.6/onnx2tf/ops/GlobalAveragePool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GlobalLpPool.py` & `onnx2tf-1.9.6/onnx2tf/ops/GlobalLpPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GlobalMaxPool.py` & `onnx2tf-1.9.6/onnx2tf/ops/GlobalMaxPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Greater.py` & `onnx2tf-1.9.6/onnx2tf/ops/Greater.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GreaterOrEqual.py` & `onnx2tf-1.9.6/onnx2tf/ops/GreaterOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/GridSample.py` & `onnx2tf-1.9.6/onnx2tf/ops/GridSample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/HardSigmoid.py` & `onnx2tf-1.9.6/onnx2tf/ops/HardSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/HardSwish.py` & `onnx2tf-1.9.6/onnx2tf/ops/HardSwish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Hardmax.py` & `onnx2tf-1.9.6/onnx2tf/ops/Hardmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Identity.py` & `onnx2tf-1.9.6/onnx2tf/ops/Identity.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/If.py` & `onnx2tf-1.9.6/onnx2tf/ops/If.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Input.py` & `onnx2tf-1.9.6/onnx2tf/ops/Input.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/InstanceNormalization.py` & `onnx2tf-1.9.6/onnx2tf/ops/InstanceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Inverse.py` & `onnx2tf-1.9.6/onnx2tf/ops/Inverse.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/IsInf.py` & `onnx2tf-1.9.6/onnx2tf/ops/IsInf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/IsNaN.py` & `onnx2tf-1.9.6/onnx2tf/ops/IsNaN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LRN.py` & `onnx2tf-1.9.6/onnx2tf/ops/LRN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LSTM.py` & `onnx2tf-1.9.6/onnx2tf/ops/LSTM.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LayerNormalization.py` & `onnx2tf-1.9.6/onnx2tf/ops/LayerNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LeakyRelu.py` & `onnx2tf-1.9.6/onnx2tf/ops/LeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Less.py` & `onnx2tf-1.9.6/onnx2tf/ops/Less.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LessOrEqual.py` & `onnx2tf-1.9.6/onnx2tf/ops/LessOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Log.py` & `onnx2tf-1.9.6/onnx2tf/ops/Log.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LogSoftmax.py` & `onnx2tf-1.9.6/onnx2tf/ops/LogSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/LpNormalization.py` & `onnx2tf-1.9.6/onnx2tf/ops/LpNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/MatMul.py` & `onnx2tf-1.9.6/onnx2tf/ops/MatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/MatMulInteger.py` & `onnx2tf-1.9.6/onnx2tf/ops/MatMulInteger.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Max.py` & `onnx2tf-1.9.6/onnx2tf/ops/Max.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/MaxPool.py` & `onnx2tf-1.9.6/onnx2tf/ops/MaxPool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/MaxUnpool.py` & `onnx2tf-1.9.6/onnx2tf/ops/MaxUnpool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Mean.py` & `onnx2tf-1.9.6/onnx2tf/ops/Mean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/MeanVarianceNormalization.py` & `onnx2tf-1.9.6/onnx2tf/ops/MeanVarianceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Min.py` & `onnx2tf-1.9.6/onnx2tf/ops/Min.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Mish.py` & `onnx2tf-1.9.6/onnx2tf/ops/Mish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Mod.py` & `onnx2tf-1.9.6/onnx2tf/ops/Mod.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Mul.py` & `onnx2tf-1.9.6/onnx2tf/ops/Mul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Multinomial.py` & `onnx2tf-1.9.6/onnx2tf/ops/Multinomial.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Neg.py` & `onnx2tf-1.9.6/onnx2tf/ops/Neg.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/NonMaxSuppression.py` & `onnx2tf-1.9.6/onnx2tf/ops/NonMaxSuppression.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/NonZero.py` & `onnx2tf-1.9.6/onnx2tf/ops/NonZero.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Not.py` & `onnx2tf-1.9.6/onnx2tf/ops/Not.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/OneHot.py` & `onnx2tf-1.9.6/onnx2tf/ops/OneHot.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Or.py` & `onnx2tf-1.9.6/onnx2tf/ops/Or.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/PRelu.py` & `onnx2tf-1.9.6/onnx2tf/ops/PRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Pad.py` & `onnx2tf-1.9.6/onnx2tf/ops/Pad.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Pow.py` & `onnx2tf-1.9.6/onnx2tf/ops/Pow.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearAdd.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearAdd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearConcat.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearConcat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearConv.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearLeakyRelu.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearLeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearMatMul.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearMatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearMul.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearSigmoid.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QLinearSoftmax.py` & `onnx2tf-1.9.6/onnx2tf/ops/QLinearSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/QuantizeLinear.py` & `onnx2tf-1.9.6/onnx2tf/ops/QuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RNN.py` & `onnx2tf-1.9.6/onnx2tf/ops/RNN.py`

 * *Files 2% similar despite different names*

```diff
@@ -645,18 +645,18 @@
         forward_bias = forward_bias_W + forward_bias_R
         fW_i = forward_weight
         fR_i = forward_recurrence_weight
         fB_i = forward_bias
         forward_kernel = tf.reshape(tf.transpose(fW_i, perm=[2, 0, 1]), shape=[input_size, -1])
         forward_recurrent_kernel = tf.reshape(tf.transpose(fR_i, perm=[2, 0, 1]), shape=[hidden_size, -1])
 
-        reverse_weight = tf.reshape(tf.convert_to_tensor(W[0]), shape=[1, hidden_size, input_size])
-        reverse_recurrence_weight = tf.reshape(tf.convert_to_tensor(R[0]), shape=[1, hidden_size, hidden_size])
-        reverse_bias_W = tf.reshape(tf.convert_to_tensor(B[0][:hidden_size]), shape=[1, hidden_size])
-        reverse_bias_R = tf.reshape(tf.convert_to_tensor(B[0][hidden_size:hidden_size*2]), shape=[1, hidden_size])
+        reverse_weight = tf.reshape(tf.convert_to_tensor(W[1]), shape=[1, hidden_size, input_size])
+        reverse_recurrence_weight = tf.reshape(tf.convert_to_tensor(R[1]), shape=[1, hidden_size, hidden_size])
+        reverse_bias_W = tf.reshape(tf.convert_to_tensor(B[1][:hidden_size]), shape=[1, hidden_size])
+        reverse_bias_R = tf.reshape(tf.convert_to_tensor(B[1][hidden_size:hidden_size*2]), shape=[1, hidden_size])
         reverse_bias = reverse_bias_W + reverse_bias_R
         rW_i = reverse_weight
         rR_i = reverse_recurrence_weight
         rB_i = reverse_bias
         reverse_kernel = tf.reshape(tf.transpose(rW_i, perm=[2, 0, 1]), shape=[input_size, -1])
         reverse_recurrent_kernel = tf.reshape(tf.transpose(rR_i, perm=[2, 0, 1]), shape=[hidden_size, -1])
```

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RandomNormal.py` & `onnx2tf-1.9.6/onnx2tf/ops/RandomNormal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RandomNormalLike.py` & `onnx2tf-1.9.6/onnx2tf/ops/RandomNormalLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RandomUniform.py` & `onnx2tf-1.9.6/onnx2tf/ops/RandomUniform.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RandomUniformLike.py` & `onnx2tf-1.9.6/onnx2tf/ops/RandomUniformLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Range.py` & `onnx2tf-1.9.6/onnx2tf/ops/Range.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Reciprocal.py` & `onnx2tf-1.9.6/onnx2tf/ops/Reciprocal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceL1.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceL1.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceL2.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceL2.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceLogSum.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceLogSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceLogSumExp.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceLogSumExp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceMax.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceMean.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceMean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceMin.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceProd.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceProd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceSum.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReduceSumSquare.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReduceSumSquare.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Relu.py` & `onnx2tf-1.9.6/onnx2tf/ops/Relu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Reshape.py` & `onnx2tf-1.9.6/onnx2tf/ops/Reshape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Resize.py` & `onnx2tf-1.9.6/onnx2tf/ops/Resize.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ReverseSequence.py` & `onnx2tf-1.9.6/onnx2tf/ops/ReverseSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/RoiAlign.py` & `onnx2tf-1.9.6/onnx2tf/ops/RoiAlign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Round.py` & `onnx2tf-1.9.6/onnx2tf/ops/Round.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ScaleAndTranslate.py` & `onnx2tf-1.9.6/onnx2tf/ops/ScaleAndTranslate.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Scatter.py` & `onnx2tf-1.9.6/onnx2tf/ops/Scatter.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ScatterElements.py` & `onnx2tf-1.9.6/onnx2tf/ops/ScatterElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ScatterND.py` & `onnx2tf-1.9.6/onnx2tf/ops/ScatterND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Selu.py` & `onnx2tf-1.9.6/onnx2tf/ops/Selu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceAt.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceAt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceConstruct.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceConstruct.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceEmpty.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceEmpty.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceErase.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceErase.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceInsert.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceInsert.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SequenceLength.py` & `onnx2tf-1.9.6/onnx2tf/ops/SequenceLength.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Shape.py` & `onnx2tf-1.9.6/onnx2tf/ops/Shape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Shrink.py` & `onnx2tf-1.9.6/onnx2tf/ops/Shrink.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sigmoid.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sign.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sin.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sinh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Size.py` & `onnx2tf-1.9.6/onnx2tf/ops/Size.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Slice.py` & `onnx2tf-1.9.6/onnx2tf/ops/Slice.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Softmax.py` & `onnx2tf-1.9.6/onnx2tf/ops/Softmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Softplus.py` & `onnx2tf-1.9.6/onnx2tf/ops/Softplus.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Softsign.py` & `onnx2tf-1.9.6/onnx2tf/ops/Softsign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SpaceToDepth.py` & `onnx2tf-1.9.6/onnx2tf/ops/SpaceToDepth.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Split.py` & `onnx2tf-1.9.6/onnx2tf/ops/Split.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/SplitToSequence.py` & `onnx2tf-1.9.6/onnx2tf/ops/SplitToSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sqrt.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sqrt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Squeeze.py` & `onnx2tf-1.9.6/onnx2tf/ops/Squeeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sub.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sub.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Sum.py` & `onnx2tf-1.9.6/onnx2tf/ops/Sum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Tan.py` & `onnx2tf-1.9.6/onnx2tf/ops/Tan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Tanh.py` & `onnx2tf-1.9.6/onnx2tf/ops/Tanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/ThresholdedRelu.py` & `onnx2tf-1.9.6/onnx2tf/ops/ThresholdedRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Tile.py` & `onnx2tf-1.9.6/onnx2tf/ops/Tile.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/TopK.py` & `onnx2tf-1.9.6/onnx2tf/ops/TopK.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Transpose.py` & `onnx2tf-1.9.6/onnx2tf/ops/Transpose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Trilu.py` & `onnx2tf-1.9.6/onnx2tf/ops/Trilu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Unique.py` & `onnx2tf-1.9.6/onnx2tf/ops/Unique.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Unsqueeze.py` & `onnx2tf-1.9.6/onnx2tf/ops/Unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Upsample.py` & `onnx2tf-1.9.6/onnx2tf/ops/Upsample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Where.py` & `onnx2tf-1.9.6/onnx2tf/ops/Where.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/Xor.py` & `onnx2tf-1.9.6/onnx2tf/ops/Xor.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/ops/_Loop.py` & `onnx2tf-1.9.6/onnx2tf/ops/_Loop.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/utils/colors.py` & `onnx2tf-1.9.6/onnx2tf/utils/colors.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/utils/common_functions.py` & `onnx2tf-1.9.6/onnx2tf/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf/utils/enums.py` & `onnx2tf-1.9.6/onnx2tf/utils/enums.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/onnx2tf.egg-info/PKG-INFO` & `onnx2tf-1.9.6/onnx2tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2tf
-Version: 1.9.5
+Version: 1.9.6
 Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
 Home-page: https://github.com/PINTO0309/onnx2tf
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -252,23 +252,23 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.5
+  ghcr.io/pinto0309/onnx2tf:1.9.6
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
-  && pip install -U onnxsim \
+  && pip install -U onnxsim==0.4.17 \
   && pip install -U simple_onnx_processing_tools \
   && pip install -U onnx2tf \
   && pip install -U h5py==3.7.0
 
   or
 
   $ pip install -e .
@@ -295,15 +295,15 @@
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1
   !sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 2
   !python3.9 -m pip install tensorflow==2.12.0 \
     && python3.9 -m pip install -U onnx \
     && python3.9 -m pip install -U nvidia-pyindex \
     && python3.9 -m pip install -U onnx-graphsurgeon \
     && python3.9 -m pip install -U onnxruntime==1.13.1 \
-    && python3.9 -m pip install -U onnxsim \
+    && python3.9 -m pip install -U onnxsim==0.4.17 \
     && python3.9 -m pip install -U simple_onnx_processing_tools \
     && python3.9 -m pip install -U onnx2tf \
     && python3.9 -m pip install -U protobuf==3.20.3 \
     && python3.9 -m pip install -U h5py==3.7.0
   ```
 
 ### 2. Run test
```

### Comparing `onnx2tf-1.9.5/onnx2tf.egg-info/SOURCES.txt` & `onnx2tf-1.9.6/onnx2tf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/setup.py` & `onnx2tf-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.5/tests/test_model_convert.py` & `onnx2tf-1.9.6/tests/test_model_convert.py`

 * *Files identical despite different names*

