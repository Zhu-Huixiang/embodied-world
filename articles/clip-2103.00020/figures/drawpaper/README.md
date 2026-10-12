# CLIP 全篇架构图

科学依据：ICML 2021正式版§2 / Fig.3，补充Tables18/20，官方CLIP模型实现。A图文数据、B双编码器、C对称配对损失、D零样本推理、E实验与局限。以ViT-B/32拆尺寸；最佳L/14@336实验在正文另讲。

`clip-imagegen-draft.png`是内置生图草稿；杯子/狗/飞机与双编码器裁片保留其视觉素材。`clip-method-v1.tex`用TikZ精排文字、公式、模块和连线，编译为PDF/PNG；上传用JPEG。`prompt.txt`保留生成指令。训练虚线更新参数，推理使用固定参数与缓存类别向量。

本图由 [DrawPaper skill](https://github.com/Zhu-Huixiang/ReadPaper/tree/main/drawpaper) 指挥 Codex，使用内置生图制作。

重编译：在本目录用XeLaTeX编译 `clip-method-v1.tex`；依赖Arial、PingFang SC字体及同目录裁片。正文公式各有独立TeX/PDF/PNG。
