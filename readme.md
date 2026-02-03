# Kuratowski 定理的严谨证明与误区纠偏

本项目提供图论中 Kuratowski 定理（平面图的充要条件）的严谨化证明流程与 TikZ 矢量示意图。

### 🚩 项目初衷

目前互联网流传的部分 Kuratowski 定理证明教程在关键逻辑上存在断层。本项目旨在通过严密的分类讨论（Case Analysis）与直观的拓扑图示，修复以下核心漏洞：
1. **收缩操作 (Contraction)** 的非平面性保持逻辑。
2. **强区间引理 (Strong Interval Lemma)** 的完备性证明。
3. 对导致 **$K_{3,3}$ 或 $K_5$** 冲突的几何交叠情况进行精确分类。

### 📂 文件说明

- **`main.tex`**: 完整的 LaTeX 源码。内嵌 31 份 TikZ 绘图代码，采用固化的坐标体系（90-330-270-210 系统）以确保拓扑关系的严谨性。
- **`Kuratowski_Proof.pdf`**: 经由 XeLaTeX 编译生成的**完整严谨证明全文**。包含全部 **25 页**的细致分类讨论、强区间引理的完备逻辑推导及全量矢量化示意图。
- **`LICENSE`**: 采用 CC BY-NC-SA 4.0 协议发布。

### 🛠 编译建议

建议使用 **XeLaTeX** 编译 `main.tex` 以获得最佳的公式与图形排版效果。

本项目推荐在 **TeX Live 2023+** 环境下编译。

1. **引擎**: 必须使用 **XeLaTeX**。它能完美支持 UTF-8 编码及中文字体。
2. **字体**: 源码依赖 `xeCJK`。请确保系统安装了相应字体，或自行在 `main.tex` 中修改 `\setCJKmainfont`。
3. **命令**:
   
   ```bash
   # 执行两次以确保 hyperref 跳转索引正确
   xelatex main.tex
   xelatex main.tex

### 📜 协议与署名

本项目采用 **[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)** 协议授权。

- **署名**: 引用或转载请注明作者为 **wibyuan**。
- **非商业**: 严禁将本项目内容用于任何盈利性目的。
- **相同方式共享**: 基于本项目的衍生作品必须以相同协议开源。

---
**参考：**
[1] 某篇具有误导性的文章：https://blog.csdn.net/m0_66201040/article/details/123440250