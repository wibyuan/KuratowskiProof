# Kuratowski & Vizing：图论基础证明

本项目目前就两个文件：

- Kuratowski 定理的基础证明。
- Vizing 定理的基础证明。

都是图论的两个重要定理，有人想要我整理出来，我就整理出来了。

## 初衷

某篇文章[1]误导人还有 5000 浏览量，我看不惯所以写了点东西。

## 文件说明

根目录有个 [main.tex](./main.tex) 和 [Kuratowski_Proof.pdf](./Kuratowski_Proof.pdf)。

想看源码就拿去看吧，31 份 TikZ 绘图源码在里面，证明 24 页，希望能帮到你。

/VizingProof 目录下也有个 [main.tex](./VizingProof/main.tex) 和 [Vizing_Proof.pdf](./VizingProof/Vizing_Proof.pdf)，道理也是一样的。

## 编译建议

建议使用 XeLaTeX 编译 `main.tex` 以获得最佳的公式与图形排版效果。

本项目推荐在 TeX Live 2023+ 环境下编译。

1. 引擎：必须使用 XeLaTeX。它能完美支持 UTF-8 编码及中文字体。
2. 字体：源码依赖 `xeCJK`。请确保系统安装了相应字体，或自行在 `main.tex` 中修改 `\setCJKmainfont`。
3. 命令：`xelatex main.tex`，复现原本效果需要再执行一次，即执行两次，这是为了确保 hyperref 跳转索引正确。

## 协议与署名

本项目采用 **[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)** 协议授权。

- 署名：你用了记得带上我的名。
- 非商业：我写它多累啊，都没想着赚钱，你别用它赚一分钱。
- 相同方式共享：你分享出来自动认定带上我设置的这个协议。

---
**参考：**
[1] 某篇具有误导性的文章：[https://blog.csdn.net/m0_66201040/article/details/123440250](https://blog.csdn.net/m0_66201040/article/details/123440250)