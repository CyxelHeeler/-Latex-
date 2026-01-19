# -Latex-
小白用AI搓的上科大毕设Latex模板

# 上海科技大学本科毕业论文 LaTeX 模板
## 模板文件结构
```
GraduationProjectLatex/
├── 0_Config/
│   └── packages.tex           # 宏包配置和格式文件
├── 1_Frontmatter/
│   ├── ShanghaiTech_Logo.png  # 校徽图片
│   ├── cover.tex              # 封面页
│   └── abstract.tex           # 中英文摘要
├── 2_Chapters/
│   ├── chapter1.tex          # 第一章
│   ├── chapter2.tex          # 第二章
│   ├── chapter3.tex          # 第三章
│   ├── chapter4.tex          # 第四章
│   ├── chapter5.tex          # 第五章
│   └── 气缸压力随曲轴转角变化的曲线.png     # 章节图片
├── 3_Backmatter/
│   ├── references.bib        # 参考文献数据库
│   └── acknowledgements.tex  # 致谢
├── main.tex                   # 主文档入口
├── README.md
└── （编译生成的辅助文件，如 .aux, .log, .pdf, .toc 等）
```

## 项目简介
本项目是基于上海科技大学官方本科毕业论文 Word 模板（下载地址：[学校官网表格模板页面](链接1)）手动制作的 LaTeX 模板。由于我编译现有的上科大毕业论文中文 LaTeX 模板（[GitHub 项目](链接2)）时总是报错，所以我根据学校 Word 模板用ai搓了一个简易版本的毕设论文模板。

模板主要依据文档《3-本科毕业论文（设计）中文模板（摘要、正文、参考文献、致谢等） - 修改版.docx》进行开发，使用 AI 辅助补充了部分内容，主打简单易用（希望如此……）。大部分格式设定集中在 `package.tex` 文件中。

## 编译方法
使用以下命令序列编译有引用的论文（需提前安装 XeLaTeX 和 BibTeX）：
```
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex”
```
