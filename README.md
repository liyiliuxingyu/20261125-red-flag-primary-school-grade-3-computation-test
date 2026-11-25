# 20261125红旗小学三年级计算测试

两份 A4 PDF 均可直接打印。题目版预留演算空间，答案版给出竖式、验算及脱式计算步骤。原卷左下的带※题采用订正后的 `603 ÷ 5`。

| 文件 | 用途 |
| --- | --- |
| [三年级计算_题目版.pdf](三年级计算_题目版.pdf) | 学生用题目版 |
| [三年级计算_答案版.pdf](三年级计算_答案版.pdf) | 教师用答案版 |
| [三年级计算.tex](三年级计算.tex) | 两个版本共用的可编辑 XeLaTeX 源码 |

## 编译 PDF

在 macOS 上可使用 MacTeX，在 Linux 上可使用 TeX Live。编译需要 XeLaTeX、TikZ、Latin Modern Math，以及简体中文思源宋体或 Fandol 宋体。

在项目目录中运行以下命令。

```sh
xelatex -halt-on-error -jobname=三年级计算_题目版 三年级计算.tex
xelatex -halt-on-error -jobname=三年级计算_答案版 '\def\AnswerEdition{}\input{三年级计算.tex}'
```
