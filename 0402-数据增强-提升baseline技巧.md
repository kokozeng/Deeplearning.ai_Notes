## 数据增强

1、垂直镜像对称

2、随机剪裁

3、色彩的转换（PCA颜色增强）

![image-20190820155121406](http://blogpicturekoko.oss-cn-beijing.aliyuncs.com/blog/2020-02-29-053354.jpg)

## 提升基准测试baseline的技巧

1、集成

独立训练几个神经网络，并平均它们的输出。

- 随机初始化三个、五个或者七个神经网络，然后训练所有这些网络，然后平均它们的输出。
- 对他们的输出进行平均计算，而不是平均他们的权重。

2、Multi-crop at test time

![image-20190820161055519](http://blogpicturekoko.oss-cn-beijing.aliyuncs.com/blog/2020-02-29-053431.jpg)

上图所示是ten-crop。

通过你的分类器来运行这十张图片，然后对结果进行平均。