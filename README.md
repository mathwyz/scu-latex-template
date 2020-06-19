# scu-latex-template

## scu-article-template

### 文本转换
很多杂志在投稿的时候要求是word格式,
这时候可以用pandoc直接进行文件格式的转换.
不仅可以转换文字,文字的格式,公式的插入,图片的插入都可以一键的转换.
非常好用.
转换完成之后,就可以稍微做一些修改就可以发表.

### NOTES
1.在转换的过程中会有些公式暂时不能识别.
比如$\,$,

2.图片会完美的插入,但是一些图片格式如.ps文件,在latex可以完美的显示,
但是在word上会显示无法识别.

3.一些不常见的包pandoc无法识别,建议使用常见的包.

4.pandoc的交叉引用是用pandoc-crossref来提供的。
我们可以用cabal来安装
sudo apt-get update
sudo apt-get install cabal-install
sudo cabal update
sudo cabal install pandoc-crossref

pandoc -o test.docx test.tex
pandoc test.tex --filter=pandoc-crossref -o test.docx 

## scu-book-template
## scu-beamer-template
## scu-cv-template
