人脸识别
========

#. [1704.06369] NormFace: L2 Hypersphere Embedding for Face Verification
    | [ `arxiv <https://arxiv.org/abs/1704.06369>`_ ] [ `code <https://github.com/happynear/NormFace>`_ ]

    本文从理论角度解释了Softmax Loss训练出来的特征为何会呈现放射形分布, 并给出了如何使用Softmax来训练归一化后的特征.

#. [1704.08063] SphereFace: Deep Hypersphere Embedding for Face Recognition
    | [ `arxiv <https://arxiv.org/abs/1704.08063>`_ ] [ `code <https://github.com/wy1iu/sphereface>`_ ]

    SphereFace是作者对自己论文Large Margin Softmax的改进, 把最后一层的权重做了归一化. 开源的代码非常扎实有参考性,
    在LFW和MegaFace任务上取得非常好的实践效果.

#. [1710.00870] Rethinking Feature Discrimination and Polymerization for Large-scale Recognition
    | [ `arxiv <https://arxiv.org/abs/1710.00870>`_ ] [ `code <https://github.com/sciencefans/coco_loss>`_ ]

    COCO loss

#. [1801.05599] Additive Margin Softmax for Face Verification
    | [ `arxiv <https://arxiv.org/abs/1801.05599>`_ ] [ `code <https://github.com/happynear/AMSoftmax>`_ ]

    之前的L-Softmax, A-Softmax引入了角间距的概念，用于改进传统的softmax loss函数，使得人脸特征具有更大的类间距和更小的类内距。
    作者在这些方法的启发下，提出了一种更直观和更易解释的additive margin Softmax (AM-Softmax)。同时，本文强调和讨论了特征正则化的重要性。
    实验表明AM-Softmax在LFW和MegaFace得到了比之前方法更好的效果。

#. [1801.07698] ArcFace: Additive Angular Margin Loss for Deep Face Recognition
    | [ `arxiv <https://arxiv.org/abs/1801.07698>`_ ] [ `code <https://github.com/deepinsight/insightface>`_ ]

    业界良心, 采用加性Margin, 开源代码中提供了相当多的工具, 不过因为是用mxnet.symbol写法来实现的, 所以对于不了解MXNet的人来说
    入门会相对困难一些, 这也是gluon-face产生的原因之一.

#. [1804.07573] MobileFaceNets: Efficient CNNs for Accurate Real-time Face Verification on Mobile Devices
    | [ `arxiv <https://arxiv.org/abs/1804.07573>`_ ] [ `code <https://github.com/moli232777144/mobilefacenet-mxnet>`_ ]

#. [1807.11649] The Devil of Face Recognition is in the Noise
    | [ `arxiv <https://arxiv.org/abs/1807.11649>`_ ] [ `code <https://github.com/fwang91/IMDb-Face>`_ ]

    ECCV'18 对于现有人脸数据集中的标签噪声问题进行了深入研究, 对MegaFace和MS-Celeb-1M数据集中的噪声特性和来源做了全面的分析, 发现干净
    子集对于提高人脸识别精度效果显著.

#. [1808.06210] GridFace: Face Rectification via Learning Local Homography Transformations
    | [ `arxiv <https://arxiv.org/abs/1808.06210>`_ ]

    通过学习局部单应变换减少人脸变形，先校正，再识别，过硬的校正技术大幅提升了人脸识别的性能. 相关实验结果已证明该方法的有效性和高效性.

#. [1810.07599] Orthogonal Deep Features Decomposition for Age-Invariant Face Recognition
    | [ `arxiv <https://arxiv.org/abs/1810.07599>`_ ]

    腾讯AI Lab发表于ECCV 2018的工作, 其目的是通过研发新的深度学习模型以提高跨年龄人脸识别的精度. 在这篇文章里, 作者提出了一种正交深度特征
    分解算法OE-CNNs, 通过把深度特征正交分解为年龄分量和身份分量, 从而将年龄分量和身份分量有效分离开, 从而提高跨年龄人脸识别精度.



..  | [ `arxiv <>`_ ] [ `code <>`_ ]




参考资料
--------

.. [1] `人脸识别的LOSS <https://zhuanlan.zhihu.com/p/34404607>`_, YaqiLYU