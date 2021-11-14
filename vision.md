## pytorch 与视觉竞赛入门

[文档地址](https://shimo.im/docs/dumrsexTRJkqSgIC/read)

#### 打卡汇总

| 任务名称                          | 难度 | 所需技能 |
| --------------------------------- | ---- | -------- |
| PyTorch张量计算与Numpy的转换      | 低   | PyTorch  |
| 梯度计算和梯度下降过程            | 低   | PyTorch  |
| PyTorch全连接层原理和使用         | 中   | PyTorch  |
| PyTorch激活函数原理和使用         | 低   | PyTorch  |
| PyTorch卷积层原理和使用           | 中   | PyTorch  |
| PyTorch常见的损失函数和优化器使用 | 中   | PyTorch  |
| PyTorch池化层和归一化层           | 中   | PyTorch  |
| 使用PyTorch搭建VGG网络            | 高   | PyTorch  |
| 使用PyTorch搭建ResNet网络         | 高   | PyTorch  |
| 使用PyTorch完成Fashion-MNIST分类  | 高   | PyTorch  |
| 使用PyTorch完成人脸关键点检测     | 高   | PyTorch  |
| 使用PyTorch搭建对抗生成网络       | 高   | PyTorch  |

#### 任务1：PyTorch张量计算与Numpy的转换

任务要点：Pytorch基础使用、张量计算

- 步骤1：配置本地Notebook环境

- 步骤2：学习Pytorch的基础语法，并成功执行以下代码

```python
c = np.ones((3,3))
d = torch.from_numpy(c)  #numpy 转tensor
```

**任务2：梯度计算和梯度下降过程**

任务要点：Pytorch梯度计算、随机梯度下降

- 步骤1：学习自动求梯度原理，https://pytorch.org/tutorials/beginner/basics/autogradqs_tutorial.html

- 步骤2：学习随机梯度下降原理，https://www.cnblogs.com/BYRans/p/4700202.html

- 步骤3：

- 使用numpy创建一个[y=10*x+b+noise(0,1)](#)的数据，其中x是0到100的范围，以0.01进行等差数列

- 使用pytroch定义w和b，并使用随机梯度下降，完成回归拟合。



**任务3：PyTorch全连接层原理和使用**

任务要点：全连接网络

- 步骤1：学习全连接网络原理，https://blog.csdn.net/xiaodong_11/article/details/82015456

- 步骤2：在pytorch中使用矩阵乘法实现全连接层

- 步骤3：在pytorch中使用nn.Linear层



**任务4：PyTorch激活函数原理和使用**

任务要点：激活函数

- 步骤1：学习激活函数的原理，https://zhuanlan.zhihu.com/p/88429934

- 步骤2：在pytorch中手动实现上述激活函数



**任务5：PyTorch卷积层原理和使用**

任务要点：卷积层

- 步骤1：理解卷积层的原理和具体使用

- https://blog.csdn.net/qq_37385726/article/details/81739179

- https://www.cnblogs.com/zhangxiann/p/13584415.html

- 步骤2：计算下如下卷积层的参数量

```Python
nn.Conv2d(
      in_channels=1,
      out_channels=32,
      kernel_size=5,    
      stride=1, 
      padding=2)
```


**任务6：PyTorch常见的损失函数和优化器使用**

任务要点：损失函数、优化器

- 步骤1：学习损失函数的细节，https://www.cnblogs.com/wanghui-garcia/p/10862733.html
- 步骤2：学习优化器的使用，https://pytorch.org/docs/stable/optim.html
- 步骤3：设置不同的优化器和学习率，重复任务2的回归过程
  - 损失函数MSE、优化器SGD、学习率0.1
  - 损失函数MSE、优化器SGD、学习率0.5
  - 损失函数MSE、优化器SGD、学习率0.01




**任务7：PyTorch池化层和归一化层**

任务要点：池化层、归一化层

- 步骤1：使用pytroch代码实现2d pool中的mean-pooling、max-pooling
  - https://pytorch.org/docs/stable/nn.html#pooling-layers

  - https://blog.csdn.net/shanglianlm/article/details/85313924

- 步骤2：学习归一化的原理，https://blog.csdn.net/qq_23981335/article/details/106572171



**任务8：使用PyTorch搭建VGG网络**

任务要点：网络搭建

https://zhuanlan.zhihu.com/p/263527295

- 步骤1：理解VGG网络的原理。

- 步骤2：使用pytorch搭建VGG网络模型。

- 步骤3：打印出VGG 11层模型 每层特征图的尺寸，以及参数量。



**任务9：使用PyTorch搭建ResNet网络**

任务要点：网络搭建

https://zhuanlan.zhihu.com/p/263526658

- 步骤1：理解ResNet网络的原理。

- 步骤2：使用pytorch搭建ResNet网络模型。

- 步骤3：打印出ResNet 18模型 每层特征图的尺寸，以及参数量。



**任务10：使用PyTorch完成Fashion-MNIST分类**

[https://github.com/masoudrostami/Fashion-MNIST-using-PyTorch/blob/main/MNIST%20Fashion%20Project.ipynb](https://github.com/masoudrostami/Fashion-MNIST-using-PyTorch/blob/main/MNIST Fashion Project.ipynb)

- 步骤1：搭建4层卷积 + 2层全连接的分类模型。

- 步骤2：在训练过程中记录下每个epoch的训练集精度和测试集精度。



**任务11：使用PyTorch完成人脸关键点检测**

数据集：[https://ai-contest-static.xfyun.cn/2021/7afa865e-5ac8-48ab-9966-d88bb33cdc15/%E4%BA%BA%E8%84%B8%E5%85%B3%E9%94%AE%E7%82%B9%E6%A3%80%E6%B5%8B%E6%8C%91%E6%88%98%E8%B5%9B_%E6%95%B0%E6%8D%AE%E9%9B%86.zip](https://ai-contest-static.xfyun.cn/2021/7afa865e-5ac8-48ab-9966-d88bb33cdc15/人脸关键点检测挑战赛_数据集.zip)

[https://gitee.com/coggle/competition-baseline/blob/master/competition/%E7%A7%91%E5%A4%A7%E8%AE%AF%E9%A3%9EAI%E5%BC%80%E5%8F%91%E8%80%85%E5%A4%A7%E8%B5%9B2021/%E4%BA%BA%E8%84%B8%E5%85%B3%E9%94%AE%E7%82%B9%E6%A3%80%E6%B5%8B%E6%8C%91%E6%88%98%E8%B5%9B/face-keypoint2.ipynb](https://gitee.com/coggle/competition-baseline/blob/master/competition/科大讯飞AI开发者大赛2021/人脸关键点检测挑战赛/face-keypoint2.ipynb)

- 步骤1：搭建4层卷积 + 2层的模型完成关键点回归。

- 步骤2：使用resnet18预训练模型完成关键点回归。



**任务12：使用PyTorch搭建对抗生成网络**

- 步骤1：学习对抗生成网络的原理，https://blog.csdn.net/DFCED/article/details/105175097

- 步骤2：学习DCGAN的代码实现，https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html

- 步骤3：使用任务11中的人脸数据（缩放至64*64），并使用DCGAN完成训练，生成人脸。