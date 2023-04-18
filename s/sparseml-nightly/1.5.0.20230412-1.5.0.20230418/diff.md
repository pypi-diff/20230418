# Comparing `tmp/sparseml_nightly-1.5.0.20230412-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.5.0.20230418-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 946339 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-Apr-12 03:01 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Apr-12 03:01 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-12 03:01 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Apr-12 03:01 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Apr-12 03:01 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Apr-12 03:01 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Apr-12 03:01 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Apr-12 03:01 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Apr-12 03:01 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Apr-12 03:01 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Apr-12 03:01 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Apr-12 03:01 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Apr-12 03:01 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-12 03:01 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-12 03:01 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4751 b- defN 23-Apr-12 03:01 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Apr-12 03:01 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-12 03:01 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Apr-12 03:01 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-Apr-12 03:01 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Apr-12 03:01 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Apr-12 03:01 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Apr-12 03:01 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Apr-12 03:01 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Apr-12 03:01 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Apr-12 03:01 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Apr-12 03:01 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Apr-12 03:01 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Apr-12 03:01 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Apr-12 03:01 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Apr-12 03:01 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Apr-12 03:01 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Apr-12 03:01 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Apr-12 03:01 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Apr-12 03:01 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Apr-12 03:01 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Apr-12 03:01 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-12 03:01 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Apr-12 03:01 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Apr-12 03:01 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Apr-12 03:01 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Apr-12 03:01 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Apr-12 03:01 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Apr-12 03:01 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Apr-12 03:01 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Apr-12 03:01 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Apr-12 03:01 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Apr-12 03:01 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Apr-12 03:01 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Apr-12 03:01 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Apr-12 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Apr-12 03:01 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41311 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31586 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Apr-12 03:01 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      734 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Apr-12 03:01 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Apr-12 03:01 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Apr-12 03:01 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Apr-12 03:01 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Apr-12 03:01 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Apr-12 03:01 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Apr-12 03:01 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Apr-12 03:01 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Apr-12 03:01 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Apr-12 03:01 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-Apr-12 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Apr-12 03:01 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Apr-12 03:01 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Apr-12 03:01 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Apr-12 03:01 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Apr-12 03:01 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-12 03:01 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Apr-12 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Apr-12 03:01 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69783 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Apr-12 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      744 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    40790 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Apr-12 03:01 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31056 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    38949 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Apr-12 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Apr-12 03:01 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Apr-12 03:01 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-12 03:01 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Apr-12 03:01 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Apr-12 03:01 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Apr-12 03:01 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Apr-12 03:01 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Apr-12 03:01 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Apr-12 03:01 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Apr-12 03:01 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Apr-12 03:01 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Apr-12 03:01 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     4390 b- defN 23-Apr-12 03:01 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19721 b- defN 23-Apr-12 03:01 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-Apr-12 03:01 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36738 b- defN 23-Apr-12 03:01 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40358 b- defN 23-Apr-12 03:01 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34464 b- defN 23-Apr-12 03:01 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Apr-12 03:01 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-Apr-12 03:01 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Apr-12 03:01 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Apr-12 03:01 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-Apr-12 03:01 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Apr-12 03:01 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-12 03:01 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Apr-12 03:01 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Apr-12 03:01 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Apr-12 03:01 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Apr-12 03:01 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Apr-12 03:01 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Apr-12 03:01 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Apr-12 03:01 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     3266 b- defN 23-Apr-12 03:01 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Apr-12 03:01 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Apr-12 03:01 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Apr-12 03:01 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx      958 b- defN 23-Apr-12 03:01 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Apr-12 03:01 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2845 b- defN 23-Apr-12 03:01 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Apr-12 03:01 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7318 b- defN 23-Apr-12 03:01 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    33189 b- defN 23-Apr-12 03:01 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2710 b- defN 23-Apr-12 03:01 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     7666 b- defN 23-Apr-12 03:01 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6298 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     2534 b- defN 23-Apr-12 03:01 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/LICENSE
--rw-rw-r--  2.0 unx    20659 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2372 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36575 b- defN 23-Apr-12 03:03 sparseml_nightly-1.5.0.20230412.dist-info/RECORD
-368 files, 3423725 bytes uncompressed, 887131 bytes compressed:  74.1%
+Zip file size: 946468 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Apr-18 03:01 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Apr-18 03:01 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-18 03:01 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Apr-18 03:01 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Apr-18 03:01 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Apr-18 03:01 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Apr-18 03:01 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Apr-18 03:01 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Apr-18 03:01 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Apr-18 03:01 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Apr-18 03:01 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Apr-18 03:01 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Apr-18 03:01 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-18 03:01 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-18 03:01 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-18 03:01 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4751 b- defN 23-Apr-18 03:01 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Apr-18 03:01 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Apr-18 03:01 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Apr-18 03:01 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-Apr-18 03:01 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Apr-18 03:01 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Apr-18 03:01 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Apr-18 03:01 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Apr-18 03:01 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Apr-18 03:01 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Apr-18 03:01 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Apr-18 03:01 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Apr-18 03:01 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Apr-18 03:01 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Apr-18 03:01 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Apr-18 03:01 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Apr-18 03:01 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Apr-18 03:01 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Apr-18 03:01 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Apr-18 03:01 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Apr-18 03:01 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Apr-18 03:01 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Apr-18 03:01 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Apr-18 03:01 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Apr-18 03:01 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Apr-18 03:01 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-18 03:01 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Apr-18 03:01 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Apr-18 03:01 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Apr-18 03:01 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Apr-18 03:01 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Apr-18 03:01 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Apr-18 03:01 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Apr-18 03:01 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Apr-18 03:01 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Apr-18 03:01 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Apr-18 03:01 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Apr-18 03:01 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Apr-18 03:01 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13274 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19634 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14520 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-Apr-18 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Apr-18 03:01 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Apr-18 03:01 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Apr-18 03:01 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Apr-18 03:01 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13002 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    41311 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31586 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Apr-18 03:01 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-Apr-18 03:01 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-Apr-18 03:01 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Apr-18 03:01 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Apr-18 03:01 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Apr-18 03:01 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Apr-18 03:01 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Apr-18 03:01 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Apr-18 03:01 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Apr-18 03:01 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Apr-18 03:01 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Apr-18 03:01 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Apr-18 03:01 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Apr-18 03:01 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10826 b- defN 23-Apr-18 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Apr-18 03:01 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Apr-18 03:01 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Apr-18 03:01 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Apr-18 03:01 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Apr-18 03:01 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-18 03:01 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Apr-18 03:01 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Apr-18 03:01 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Apr-18 03:01 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-18 03:01 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Apr-18 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Apr-18 03:01 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Apr-18 03:01 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Apr-18 03:01 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Apr-18 03:01 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69783 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Apr-18 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      744 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    40790 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Apr-18 03:01 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31056 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Apr-18 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Apr-18 03:01 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Apr-18 03:01 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-18 03:01 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Apr-18 03:01 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Apr-18 03:01 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Apr-18 03:01 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Apr-18 03:01 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Apr-18 03:01 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Apr-18 03:01 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Apr-18 03:01 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Apr-18 03:01 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Apr-18 03:01 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Apr-18 03:01 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Apr-18 03:01 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Apr-18 03:01 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     4390 b- defN 23-Apr-18 03:01 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    19721 b- defN 23-Apr-18 03:01 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30936 b- defN 23-Apr-18 03:01 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36738 b- defN 23-Apr-18 03:01 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40358 b- defN 23-Apr-18 03:01 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34464 b- defN 23-Apr-18 03:01 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Apr-18 03:01 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Apr-18 03:01 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-Apr-18 03:01 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Apr-18 03:01 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Apr-18 03:01 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-18 03:01 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Apr-18 03:01 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-Apr-18 03:01 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Apr-18 03:01 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Apr-18 03:01 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-Apr-18 03:01 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Apr-18 03:01 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-18 03:01 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Apr-18 03:01 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Apr-18 03:01 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Apr-18 03:01 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Apr-18 03:01 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Apr-18 03:01 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Apr-18 03:01 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Apr-18 03:01 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     3266 b- defN 23-Apr-18 03:01 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Apr-18 03:01 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Apr-18 03:01 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Apr-18 03:01 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx      958 b- defN 23-Apr-18 03:01 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Apr-18 03:01 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2845 b- defN 23-Apr-18 03:01 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Apr-18 03:01 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7318 b- defN 23-Apr-18 03:01 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    33460 b- defN 23-Apr-18 03:01 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2710 b- defN 23-Apr-18 03:01 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     7694 b- defN 23-Apr-18 03:01 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Apr-18 03:01 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6298 b- defN 23-Apr-18 03:01 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     2534 b- defN 23-Apr-18 03:01 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    20659 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2372 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36575 b- defN 23-Apr-18 03:03 sparseml_nightly-1.5.0.20230418.dist-info/RECORD
+368 files, 3424359 bytes uncompressed, 887260 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/LICENSE
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/METADATA
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/NOTICE
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/WHEEL
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230412.dist-info/RECORD
+Filename: sparseml_nightly-1.5.0.20230418.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/pytorch/utils/helpers.py

```diff
@@ -96,14 +96,15 @@
     "get_layer_param",
     "set_deterministic_seeds",
     "torch_distributed_zero_first",
     "thin_model_from_checkpoint",
     "MEMORY_BOUNDED",
     "memory_aware_threshold",
     "download_framework_model_by_recipe_type",
+    "detach",
 ]
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 ##############################
@@ -1158,7 +1159,18 @@
 
     if framework_model is None:
         # fetching the model for inference or fall back if model.ckpt.pth doesn't exist
         model_name = f"model.{model_suffix}"
         framework_model = zoo_model.training.default.get_file(model_name)
 
     return framework_model.path
+
+
+def detach(x: Union[torch.Tensor, List, Tuple]):
+    if isinstance(x, torch.Tensor):
+        return x.detach()
+    elif isinstance(x, List):
+        return [detach(e) for e in x]
+    elif isinstance(x, Tuple):
+        return tuple([detach(e) for e in x])
+    else:
+        raise ValueError("Unexpected type to detach")
```

## sparseml/yolov8/trainers.py

```diff
@@ -523,18 +523,19 @@
 
 class SparseYOLO(YOLO):
     def __init__(self, model="yolov8n.yaml", type="v8") -> None:
         model_str = str(model)
 
         if model_str.startswith("zoo:"):
             model = download_framework_model_by_recipe_type(
-                Model(model_str), model_suffix=".pt"
+                Model(model_str), model_suffix="pt"
             )
             self.is_sparseml_checkpoint = True
-        elif model_str.endswith(".pt"):
+
+        if model_str.endswith(".pt"):
             if os.path.exists(model_str):
                 ckpt = torch.load(model_str)
                 self.is_sparseml_checkpoint = (
                     "source" in ckpt and ckpt["source"] == "sparseml"
                 )
             else:
                 self.is_sparseml_checkpoint = False
@@ -582,16 +583,22 @@
             (
                 self.ModelClass,
                 self.TrainerClass,
                 self.ValidatorClass,
                 self.PredictorClass,
             ) = self._assign_ops_from_task(self.task)
 
-            self.model = self.ModelClass(dict(self.ckpt["model_yaml"]))
-            if "recipe" in self.ckpt:
+            if "yaml" in self.ckpt:
+                self.model = self.ModelClass(dict(self.ckpt["yaml"]))
+            elif "model_yaml" in self.ckpt:
+                self.model = self.ModelClass(dict(self.ckpt["model_yaml"]))
+            else:
+                self.model = self.ModelClass(dict(self.ckpt["model"].yaml))
+
+            if "recipe" in self.ckpt and self.ckpt["recipe"]:
                 manager = ScheduledModifierManager.from_yaml(self.ckpt["recipe"])
                 epoch = self.ckpt.get("epoch", -1)
                 if epoch < 0:
                     epoch = float("inf")
                 LOGGER.info(
                     "Applying structure from sparseml checkpoint "
                     f"at epoch {self.ckpt['epoch']}"
```

## sparseml/yolov8/validators.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 import json
 
 import torch
 from tqdm import tqdm
 
+from sparseml.pytorch.utils import detach
 from ultralytics.nn.autobackend import AutoBackend
 from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.yolo.engine.validator import BaseValidator
 from ultralytics.yolo.utils import TQDM_BAR_FORMAT, callbacks, emojis
 from ultralytics.yolo.utils.checks import check_imgsz
 from ultralytics.yolo.utils.ops import Profile
 from ultralytics.yolo.utils.torch_utils import de_parallel, select_device
@@ -132,15 +133,15 @@
 
             # pre-process predictions
             with dt[3]:
                 preds = self.postprocess(preds)
 
             # During QAT the resulting preds are grad required, breaking
             # the update metrics function.
-            detached_preds = [p.detach() for p in preds]
+            detached_preds = detach(preds)
             self.update_metrics(detached_preds, batch)
 
             if self.args.plots and batch_i < 3:
                 self.plot_val_samples(batch, batch_i)
                 self.plot_predictions(batch, detached_preds, batch_i)
 
             self.run_callbacks("on_val_batch_end")
```

## Comparing `sparseml_nightly-1.5.0.20230412.dist-info/LICENSE` & `sparseml_nightly-1.5.0.20230418.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230412.dist-info/METADATA` & `sparseml_nightly-1.5.0.20230418.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.5.0.20230412
+Version: 1.5.0.20230418
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
```

## Comparing `sparseml_nightly-1.5.0.20230412.dist-info/NOTICE` & `sparseml_nightly-1.5.0.20230418.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt` & `sparseml_nightly-1.5.0.20230418.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230412.dist-info/RECORD` & `sparseml_nightly-1.5.0.20230418.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
 sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
 sparseml/pytorch/utils/benchmarker.py,sha256=Zw1pEj7wDe4ZU_-G0JOCymdLXydN19K1QZKzPJvBp9E,9706
 sparseml/pytorch/utils/callbacks.py,sha256=1z10T8xE0IY5mcL2ARSsHDt6sDWRVF-Nq6zVf9OvD0s,2846
 sparseml/pytorch/utils/distributed.py,sha256=lJtEvgMg6LvH9iUwhveCaWNrx_t7pjn-sOW9rfYViwI,1061
 sparseml/pytorch/utils/exporter.py,sha256=KfoPciN46ZDHKgvVk7oYBR_cyZwihRPNcCm-EvPnpfg,31056
-sparseml/pytorch/utils/helpers.py,sha256=QF4TobigcGoFG6kCKw7U8BneHESMQu7yNJhxQGAXS5M,38949
+sparseml/pytorch/utils/helpers.py,sha256=pCQMNjgVQN4jYuerj_6YJKGDFmOZ8-3eJMcLEw5V6-A,39284
 sparseml/pytorch/utils/log_sparsification_info.py,sha256=o9WdrrDU8W1J09NHLnW2cja5PXNq442UFzgpXf8po8M,1663
 sparseml/pytorch/utils/logger.py,sha256=KOhmFXNj46gmy5XovwQOZigBuHidVmNqDnVWMUXD7PE,31374
 sparseml/pytorch/utils/loss.py,sha256=RWFyThMBaB-7jAVuS3_CU5bmsWOVFG1jqzPciSpVsj8,27048
 sparseml/pytorch/utils/model.py,sha256=KCEZ6cNkIzLKd6N8KqJe7GX3GD-PoWErZk05nEbQuJc,11754
 sparseml/pytorch/utils/module.py,sha256=gWKNLqn8bI_q97u_QC95WkxBPAclMCwz3HmrZEHEYtU,39117
 sparseml/pytorch/utils/sparsification.py,sha256=BbH3ePC74YWGddSoLcSenLd0D_0nz-Xk5vx4Ui_KkzY,8809
 sparseml/pytorch/utils/ssd_helpers.py,sha256=05fySE5KNwrt7UF213niHp2STRSeprlU1NbLAjpYRaU,30059
@@ -349,20 +349,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=4akRvqiJRrRI9kcdXG3rqIiZLWIh7tvA-0zOI2zxO0w,958
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=e6BT4CsAgtm-RIn3eyCsMqxVvRp9XuY71pS12vVMOLc,2845
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=UKUkpTGaUZ76wRz8w0Rsgi3o9XvsTxdcJ5nmXKOvtkA,7318
-sparseml/yolov8/trainers.py,sha256=s7vfeAyyAVRfaZTgOf9BVd44pOIfnUcjAeHX3w0RwEw,33189
+sparseml/yolov8/trainers.py,sha256=AB6FAXmrZvb-kYnnIYU9HP3iBsvqzEq1HA4G8t9eP-0,33460
 sparseml/yolov8/val.py,sha256=E1mzjay7F1ErOoqTptBmj9JR310pRu5PI3jp1YVDpH0,2710
-sparseml/yolov8/validators.py,sha256=A65KT1a0SZCGKqsaJufxUHrzsvJsd7VBJbRt3O5aC84,7666
+sparseml/yolov8/validators.py,sha256=Zdr68iqk_1uyiPI5-3bjs2Jv1DmibkNQh9MznTy7bFk,7694
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=YbiV_0cv_W0xrhtZLg6ActLeSRYYikrOzHz0FqJ0LII,6298
 sparseml/yolov8/utils/helpers.py,sha256=P6RyXxq6pyorWlsdcfRy8i_ncezCpvwQNIsXE7vDFSM,2534
-sparseml_nightly-1.5.0.20230412.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.5.0.20230412.dist-info/METADATA,sha256=Er83gTenbV7VOQfPgoHnUx31JuRGwWEVSqDziWBu2b8,20659
-sparseml_nightly-1.5.0.20230412.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.5.0.20230412.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.5.0.20230412.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
-sparseml_nightly-1.5.0.20230412.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.5.0.20230412.dist-info/RECORD,,
+sparseml_nightly-1.5.0.20230418.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.5.0.20230418.dist-info/METADATA,sha256=eXlAM5AyKDuVCEL21YgLJprhBakA-KhNPzBvt83e-Yc,20659
+sparseml_nightly-1.5.0.20230418.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.5.0.20230418.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.5.0.20230418.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
+sparseml_nightly-1.5.0.20230418.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.5.0.20230418.dist-info/RECORD,,
```

