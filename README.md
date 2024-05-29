# midterm-2
首先安装所需的 Python 库：主要使用了 torch torchvision，mmcvfull，mmdet 三个库
mmdet_root=~/mmdetection # 将 配 置 文 件 修 改 为 实 际 的
mmdetection 安装目录
以及安装了 PyTorch 和 CUDA
一、 Faster R-CNN 配置文件
运行 python 代码配置 Faster R-CNN 进行训练
数据集划分
训练集：VOC2007和VOC2012的trainval数据集
测试集：VOC2007的test数据集
网络结构
Faster R-CNN：基于ResNet-50的特征提取网络
YOLO V3：基于Darknet-53的特征提取网络
超参数设置
Batch size：2
Learning rate：0.02（Faster R-CNN），0.001（YOLO V3）
优化器：SGD
Epochs：12（Faster R-CNN），50（YOLO V3）
Loss function：包含分类损失和边界框回归损失
评价指标：mAP（mean Average Precision）
