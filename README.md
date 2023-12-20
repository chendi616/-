# AutoDocx程序使用手册
## 一、使用方法（省流）
1. 将需要转换的文本粘贴至`input.txt`。
⚠️ 请勿对`module.docx`进行任何内容或路径的改动。保证`input.txt`、`module.docx`、`AutoDocx.exe`三个文件在同一目录下。

2. 双击`AutoDocx.exe`在当前路径下生成`标题.docx`标准格式公文。
⚠️ 程序生成的`标题.docx`可能是一个[只读文件](https://zhuanlan.zhihu.com/p/96568824)，只需另存为一个新文件即可。如无此情况，请忽略此条。

3. 请人工复核文件的格式。
---
## 二、详细说明（可以不看）
<aside>
💡 以下为详细说明，包含各文件的详细用途、注意事项、作用成效，没时间可以不看。

</aside>

### 1. 输入文件`input.exe`

**输入要求：**

- 无需考虑格式要求，直接在`input.txt`中编写内容，或将文字内容复制进`input.txt`。
- 标题最好写在一行，而不是分成两行，便于标题识别。后续可手动给标题换行。

**在input.txt中，您无需考虑：**

- 段落首部的缩进。无需在段落前添加或者删除缩进，程序会自动判断此段需要缩进还是顶格。
- 段落间多余的换行。无需手动处理多余的空行，程序会自动删除多余的换行符。若两个句子之间没有换行，则视为同一段落。
- 文字间多余的空格。程序会自动删除文字间的一个或多个空格，但同样会删除英文之间的空格。如`Hello World -> HelloWorld`。
- 半角符号问题**。**程序会自动将所有半角符号`,;:!?()`替换成全角符号`，；：！？（）`，但是请勿将句号`。`写成半角形式`.`。

### 2. 固定文件`Module.exe`

充当页面布局的模版作用，无需使用且不得更改此文档的内容及路径。

### 3. 可执行文件`AutoDocx.exe`

双击`AutoDocx.exe`即可运行程序，在当前路径下生成`标题.docx`标准格式公文。
⚠️注意：请务必将`input.txt`、`module.docx`、`AutoDocx.exe`三个文件放在同一目录下。

### 4. 输出文件`标题.docx`

**标准格式：**

- 页面布局

> 页边距：顶部3.7cm，底部3.5cm，左右两侧2.8cm。
纸张尺寸：A4（20.99cm*29.7cm）。
页码：已按要求预处理。
> 
- 标题

> 格式：华文中宋、二号、加粗、居中。
标题下端按二号字空一行。
如需排列成梯形格式需手动换行。
> 
- 正文

> 格式：仿宋、三号、行距固定值30磅。
若正文首段是XX单位：，则此行顶格，否则段首缩进。
第一层标识：若正文某一段落以一、、二、等开头，则视为第一层标识，置黑体三号。
第二层标识：若正文某一段落以（一）、（二）等开头，则视为第二层标识，置楷体三号。
第三、四层标识：第三层标识1.、第四层标识（1）与常规正文格式相同，不另作处理。
附件、联系人：格式与正文相同，与正文间隔一行。需注意若附件名字较长，回行后需手动与上一行附件名称首字对齐。
> 
- 落款

> 格式与正文相同。
前置空格，顶至最右，需手动调整空格及与正文间的距离。
> 

**您可能需要手动调整：**

- **标题**如需排列成梯形格式。
- **附件**名如较长回行后需手动与上一行附件名称首字对齐
- **落款**默认顶至最右，需手动微调位置。

