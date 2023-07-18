# Collection-of-papers-and-codes
| [2023](#2023) | [2022](#2022) | [2021](#2021) | [2020](#2020) | [2019](#2019) | 
|:-------:|:-------:|:-------:|:-------:|:-------:|

## conference

## 2023

| Title | Description | Conf | Code | 
|:--------|:--------:|:--------:|:-------:|
| [PEFAT: Boosting Semi-supervised Medical Image Classification via Pseudo-loss Estimation and Feature Adversarial Training](https://openaccess.thecvf.com/content/CVPR2023/papers/Zeng_PEFAT_Boosting_Semi-Supervised_Medical_Image_Classification_via_Pseudo-Loss_Estimation_and_CVPR_2023_paper.pdf) | 半监督学习中的伪标签方法已被证明在计算机视觉和医学成像中是有效的。目前大多数工作都致力于从模型预测概率的角度来寻找具有高可信度伪标签的样本。然而，如果没有仔细调整概率阈值，这种方式可能会导致包含大量的错误的伪标签数据。此外，低置信度的样本经常被忽视，并没有充分利用其潜力。在本文中，我们提出了一种新的伪损失估计和特征对抗训练的半监督框架，从损失分布建模和对抗训练的角度来提高半监督医学图像分类的性能。实验结果表明，我们的方法能够有效地提高半监督场景下的医学图像多标签、多分类能力。该成果已经被CVPR2023接收。| CVPR | [code](https://github.com/maxwell0027/PEFAT) | 
| [Devil is in Channels: Contrastive Single Domain Generalization for Medical Image Segmentation](https://arxiv.org/abs/2306.05254) | 由于不同医疗中心的医学图像成像质量存在不一致的现象，基于深度学习的医学图像分割模型在部署到新的医疗中心时会出现性能下降的问题。目前解决这个问题的方法有无监督域适应方法与多源域泛化方法，但是这些方法往往需要来自多个医疗中心的数据同时训练医学图像分割模型，存在隐私泄漏的风险。相比这些方法，单源域泛化只需要来自单个医疗中心的数据训练模型，可以减少隐私泄漏的风险。本文提出了一种基于特征通道层面对比学习的单源域泛化方法（CCSDG）用于医学图像分割。在CCSDG中，我们将原始医学图像进行风格相关的数据增广增广出不同风格的图像，利用浅层CNN从这些图像中提取特征，并用于对比训练，从而将结构相关的特征和风格相关的特征进行显式的解耦，而只将结构相关的特征用于分割任务。我们在多中心视杯视盘分割数据集上对我们的方法进行了验证，并对比了6种流行的单源域泛化方法。实验结果证明了我们的CCSDG中每个模块的有效性，并且CCSDG的性能超过了其他的单源域泛化方法。 | MICCAI | [code](https://github.com/ShishuaiHu/CCSDG) |
| [Transformer-based Annotation Bias-aware Medical Image Segmentation](https://arxiv.org/abs/2306.01340) | 医学图像分割的人工标注是主观的，标注结果不可避免地受到标注者相关偏差的影响，这种标注偏差会被深度学习方法所模拟或放大。近年来，研究人员提出这种偏差是由标注者偏好和随机误差两部分组成，分别由解码器后的卷积层和像素独立的高斯分布建模。卷积层难以有效地模拟全分辨率水平上不同程度的偏好。此外，像素独立的高斯分布忽略了像素间的相关性，导致分割边界不连续。本文提出了一种基于Transformer的标注偏差感知医学图像分割模型，通过建模标注者偏好和随机误差来解决标注偏差。该模型采用带有可学习查询向量的Transformer来提取不同偏好的标注者关注的特征。这使得模型能够使用单个分割头同时产生多个具有不同偏好的分割结果。此外，该模型采用多变量正态分布假设建模像素相关性，并学习标注分布以分离出随机误差。我们在由六个标注者注释的视杯视盘分割数据集上评估了模型性能。结果表明，该模型优于现有考虑标注偏差的其他医学图像分割模型。 | MICCAI | [code](https://github.com/Merrical/TAB) |
