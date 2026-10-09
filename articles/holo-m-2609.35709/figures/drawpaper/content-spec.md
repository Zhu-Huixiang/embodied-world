# Holo-M DrawPaper 内容规格

来源：arXiv 2609.35709v1，完整12页已读，无另附附录；方法§3，Table1，Fig1/2/3，§4.5。PDF SHA256 fedcfc74ba23e5e6af0d414d00ae792b7b1be961ff291272aa266e09dd715431。

| 模块/位置 | 输入与内部计算 | 输出/连线 | 依据 |
|---|---|---|---|
| 训练带 | EgoDex只有EEF；HE及SIMPLE只监督样本可用组；missing groups不计loss | AR预训练→SIMPLE对齐→去mask微调→可选单任务 | p3/7 §3.1/3.4，Fig2 |
| token带 | 30×96表示，4组48/29/14/5维；每维2个DCT低频系数，4级RVQ残差 | 100/62/32/14 tokens，共208；结构token另计 | p4 Table1，Eq5–8 |
| 推理带 | 图像、task、setup、量化state进入Qwen3-VL-2B，视觉encoder训练固定，语言backbone更新 | 当前组双向注意力、跨组因果；按置信度去mask；前缀与已完成组缓存 | p5/6 Eq9,11–13 |
| 解码带 | EEF→body→hand→kin，组内并行；8轮×4组 | 连续目标，经WBC执行；EEF为训练共享表征，非额外电机组 | p3/6 Fig1, §3.1/3.3 |
| 时钟带 | 每500ms观测，1秒chunk；旧chunk在推理期间执行 | 后续chunk丢弃hold内前段，接管后段 | p10 Fig3 §4.5 |

核心数学：Lg=2Dg+4；208=2×96+4×4。顺序深度为32，208/32=6.5；实测推理延迟详见正文。损失详细公式放在阅读记录，不在手机版挤入全损失；本图以数据可用性和更新阶段表达训练逻辑。

计划：内置imagegen草稿→核验→单页XeLaTeX/TikZ终稿。草稿顶部机器人/token插画用graphicx裁切保留，训练/推理/时钟主体为可编辑文字、token网格和连线。不是把整图嵌入PDF。图内保留科学内容，制作署名和 skill 仓库链接放在图旁。

不确定：未公开代码，不能确定部署是否为效率省去辅助EEF组；图仅照论文四组canonical decoding讲解，不补实现细节。96维是重叠表示，非96个电机。超预算行为沿用作者描述，不扩写成安全保证。
