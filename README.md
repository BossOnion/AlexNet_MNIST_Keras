# AlexNet_MNIST_Keras
基于TensorFlow框架和Keras库搭建AlexNet模型，使用MNIST数据集进行训练，并进行了int8量化。  
【keras_alexnet.ipynb】使用GPU进行模型训练  
【tflite_alexnet.ipynb】使用CPU进行模型转换、量化和测试  
【alexnet.h5】使用GPU训练后保存的模型，使用h5格式，大小为667MB  
【alexnet.tflite】使用CPU转化成tflite格式的模型，大小为222MB  
【alexnet_quanitfied.tflite】对原h5格式模型进行int8量化后转化为tflite格式，激活值（偏置）为float32、权重为int8，大小为55.6MB  
【mnist.npz】本地MNIST数据集  
【handwrite_num】用于测试的10张手写数字图片  
本次工程主要是验证了使用Keras搭建AlexNet模型、使用TfLite转化、量化AlexNet模型，取得了不错的模型压缩效果。  
