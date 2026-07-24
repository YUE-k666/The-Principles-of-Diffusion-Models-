# 扩散模型的原理（中文版）

> 本仓库是 [The Principles of Diffusion Models](http://arxiv.org/abs/2510.21890)（arXiv:2510.21890）的**中文翻译版**，含完整 LaTeX 源码与编译好的 PDF。

原书由 **Chieh-Hsin Lai、Yang Song、Dongjun Kim、Yuki Mitsufuji、Stefano Ermon** 著，系统阐述了扩散模型（Diffusion Models）的核心原理，追溯其起源，并统一了变分、分数、流三大视角。

## 内容简介

- **第一部分（A）**：深度生成式建模导论
- **第二部分（B）**：扩散模型的起源与基础——变分视角（VAE→DDPM）、分数视角（EBM→NCSN→Score SDE）、流视角（NF→Flow Matching）、三者等价性、最优传输与扩散模型
- **第三部分（C）**：扩散模型的采样——引导（Guidance）、高级数值求解器
- **第四部分（D）**：迈向学习快速的扩散生成器——蒸馏方法、从零学习流映射
- **结语与展望**：超越连续状态空间的扩散
- **附录**：微分方程速成、连续性方程、随机微分方程与 Itô 微积分、证明

## PDF

编译好的中文版 PDF 位于：[`扩散模型的原理_中文版.pdf`](./扩散模型的原理_中文版.pdf)（约 512 页）。

## 如何编译

本项目使用 **XeLaTeX** 编译（中文需要 XeLaTeX + xeCJK）：

```bash
xelatex main_v2
biber main_v2
xelatex main_v2
xelatex main_v2
```

### 字体依赖

需要安装 **Noto Serif CJK SC** 与 **Noto Sans CJK SC** 字体（Google Noto 字体族），用于中文渲染。

### 翻译说明

- 全部正文、章节标题、图表标题、定理环境名称均已译为简体中文。
- 所有数学公式、LaTeX 命令、交叉引用、参考文献条目（作者、标题）保持原文不变。
- 技术术语采用中英对照（如“扩散模型（Diffusion Model）”），首次出现时附英文。
- 参考文献保留英文（学术规范）。

## 致谢与版权

本中文翻译仅供学习研究之用，版权归原书作者及出版方（MIT Press / Now Publishers）所有。

原书项目主页：<https://the-principles-of-diffusion-models.github.io/>
