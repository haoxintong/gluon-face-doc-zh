Datasets
========

``gluonfr.data`` 提供了训练和验证的输入流程, 目前所有数据集由洞见实验室制作提供, 所有人脸图像均使用MTCNN进行对齐,
并截断至``(112, 112)``大小. 为了加速读取它们被转化成 ``train.rec``, ``train.idx`` 以及
``val_data.bin``, 详细信息请参考
`[insightface/Dataset-Zoo] <https://github.com/deepinsight/insightface/wiki/Dataset-Zoo>`__.

在 ``examples/dali_utils.py`` 文件中, 有一个使用Nvidia DALI准备数据的简单例子, 当CPU处理数据成为训练瓶颈时推荐使用.

将下载好的数据集按如下结构组织:

::

    face/
        emore/
            train.rec
            train.idx
            property
        ms1m/
            train.rec
            train.idx
            property
        lfw.bin
        agedb_30.bin
        ...
        vgg2_fp.bin

为了保持和MXNet一致, 使用 ``~/.mxnet/datasets`` 作为数据集的根目录.

参考文献
^^^^^^^^

- LFW
    `"Labeled Faces in the Wild: A Database for Studying Face Recognition in Unconstrained Environments"
    <http://vis-www.cs.umass.edu/lfw/lfw.pdf>`__

- CALFW
    `"A Database for Studying Cross-Age Face Recognition in Unconstrained Environments"
    <http://arxiv.org/abs/1708.08197>`__

- CPLFW
    `"Cross-pose LFW: A database for studying cross-pose face recognition in unconstrained environments"
    <http://www.whdeng.cn/CPLFW/Cross-Pose-LFW.pdf>`__

- CFP_fp, CFP_ff
    `"Frontal to Profile Face Verification in the Wild" <http://www.cfpw.io/paper.pdf>`__

- AgeDB_30
    `"AgeDB: the first manually collected, in-the-wild age database"
    <https://ibug.doc.ic.ac.uk/media/uploads/documents/agedb.pdf>`__

- VGG2_fp
    `"VGGFace2: A dataset for recognising faces across pose and age"
    <https://arxiv.org/abs/1710.08092>`__
