# 本篇方法链路 · MAE

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

[本篇星系](../mae.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/mae.md) · [原文依据](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)
