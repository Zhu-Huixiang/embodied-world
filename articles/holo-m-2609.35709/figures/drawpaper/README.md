# Holo-M 的 DrawPaper 配图

本图由 [DrawPaper skill](https://github.com/Zhu-Huixiang/ReadPaper/tree/main/drawpaper) 指挥 Codex，使用内置生图制作。

终稿使用内置生图草稿中的概念机器人插画，方法文字、公式、训练/推理连线及控制时钟由 TikZ 独立排版。图中的时钟带讲解推理与执行如何衔接。

- [论文原图 Fig. 1](../original/fig1-original.png)：原始整体架构，arXiv v1 PDF 第 3 页。
- [论文原图 Fig. 3](../original/fig3-original.png)：原始部署时序，arXiv v1 PDF 第 10 页；[原图局部](../original/fig3-takeover-original-detail.png)仅裁切放大接管区域。
- [选定生图草稿](holo-m-imagegen-draft.png)：实际生成素材，未经科学精排的独立对照材料。
- [终稿 PNG](holo-m-method-v2.png)、[单页 PDF](holo-m-method-v2.pdf)、[TikZ 源码](holo-m-method-v2.tex)：经过科学与视觉核对的混合排版终稿。
- [实际提示词](prompt.txt)、[科学内容规格](content-spec.md)：来源与图中模块对应关系。

重编译时将本目录保留完整，用 XeLaTeX 编译 holo-m-method-v2.tex。源码引用同目录生图草稿；不需要联网调用生图 API。源码字体设置为 macOS PingFang SC 与 Helvetica；PDF 内字体名称可能显示为 PingFangHK。其他系统需在源码 fontspec/xeCJK 设置处替换为已安装的中英文字体，再重新核验换行和遮挡；本包不分发字体文件。
