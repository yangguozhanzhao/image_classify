# 摄像头动态二/多分类应用

## 1. 软件功能

* 在树莓派（mac或者win）利用摄像头实现：
  * 实时录入训练数据集（二分类或者多分类）
  * 本机进行训练并保存模型
  * 摄像头录入样本，利用训练的模型进行预测

* 先在mac上开发，然后移植到树莓派，好用则移植到iOS平台，统一使用tensorflow

## 2.软件构想

* 界面tkinter+opencv+tensorflow（或者sklearn,如果可以）
* 模型结构使用最简单的，后续允许选择
* 训练好的模型保存，可以动态选择

## 3.测试记录

* 三类分类+lenet模型,a类为OK，b类为NG，C类为没有被测物体
  * a类200,b类一种不良200,c类100,测试效果比较好
  * 镜头对准被测物体，被测物体多移动
  * 应用到单路接收器上基本没有问题