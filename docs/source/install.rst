Installation
------------
尽管此工程理论上能够在Windows系统上使用, 但我们还是建议使用ubuntu系统进行学习和开发.

Gluon Face 支持Python 3.5及以上版本. 为了安装此工具包, 首先安装MXNet和gluon-cv:

.. code:: shell

    pip install gluoncv --pre
    pip install mxnet-mkl --pre --upgrade
    # if cuda XX is installed
    pip install mxnet-cuXXmkl --pre --upgrade

然后安装此项目:

-  从源码安装(推荐)

.. code:: shell

    pip install git+https://github.com/THUFutureLab/gluon-face.git@master

-  使用pip

.. code:: shell

    pip install gluonfr
