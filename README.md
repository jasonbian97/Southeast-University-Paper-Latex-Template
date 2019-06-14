

# 文档结构

- Main.tex : 主文件入口，对应生成main.pdf 文件
- thuthesis.pdf 模板说明文件
- Thuthesis.dtx 模板实现文件，如果想要自定义样式在此处修改，与thuthesis.pdf对应。更新Thuthesis.dtx后，执行 $xetex thuthesis.ins 可以生成新的Thuthesis.cls文件，供main.tex 调用
- /data/ : 存放各章节的tex文件
- /figures/ : 图片文件
- /ref/ : *.bib

# 使用方法

打开main.tex 文件，使用xelatex编译器进行编译；

生成完整的(带有正确引用编号)的文件，使用四次编译：xelatex->bibtex->xelatex->xelatex

技巧：解决编译速度很慢：假如正在写第二章，则可以在main.tex 中将其他章节先注释掉。

# 升级

## 
从 [GitHub](https://github.com/xueruini/thuthesis) 下载放入论文目录，执行命令（Windows 用户在文件夹空白处按`Shift+鼠标右键`，点击“在此处打开命令行窗口”）：

    xetex thuthesis.ins

即可得到 `thuthesis.cls` 等模板文件。

# 引用

> 基于 https://github.com/xueruini/thuthesis 修改

# 特别说明

封面需要在生成mian.pdf后手动替换。















