# 北京航空航天大学硕博学位论文LaTeX模板4.0.0

从北航官方学位论文latex模板4.0.0版本修改的。原学位论文模板链接：
https://bhpan.buaa.edu.cn/link/AA047BF1DD55A54A40A86244882B24FDF4


以下是原学位论文模板的readme，常见问题通过阅读readme和模板中的注释部分基本可以得到解决。

## 模板使用
1. 参考下方 `环境配置` 部分配置 `LaTeX` 写作环境
2. 参考下方 `写作提示` 部分撰写论文

## 环境配置

常见的 `LaTeX` 写作环境有两种，一种是使用 Overleaf 的在线环境，另一种是使用 `TexLive` 的本地环境。两种写作环境各有优劣：
- 在线环境基本无需配置，本地环境需要较复杂的配置
- 在线环境的免费账户有着**严苛**的编译时长限制，类似毕业论文这样的长篇文章**基本不可能**通过编译，需要开通订阅才能解锁编译时长限制

### 1. Overleaf 环境

将项目压缩包上传至 [Overleaf](https://cn.overleaf.com/) 后，修改编译选项为 `XeLaTeX` 即可开始写作。

### 2. 本地编译环境

编译环境请选择 'TexLive' + ‘Texstdio' 方案

#### 2.1 TexLive安装

- MacOS用户点击 [MacTeX](https://mirror.ctan.org/systems/mac/mactex/MacTeX.pkg) 下载并安装 `MacTex` 即可（这是一个包含了`TexLive` 环境的程序）
- Windows 和 Linux 用户需要参考以下步骤安装 `TexLive+TexStdio`

1. 前往 [TexLive Images - 清华大学开源软件镜像站](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/) 下载 `texlive.iso` 安装包
2. 装载 `texlive.iso` 后，Windows 用户点击 `install-tl-windows.exe` 启动安装程序，Linux 用户请使用`sudo install-pl`启动安装
3. 修改安装路径（否则默认安装在系统盘，会占据巨大的系统空间！）
4. 点击 `安装`，等待漫长的安装过程（可能会持续几十分钟）
5. 安装结束后，使用终端输入 `tex`，出现下方结果即表示安装成功

具体详细的安装步骤可前往 https://blog.csdn.net/qq_43431934/article/details/124079142
注意！！！！
在安装之后，需要在计算机的环境变量Path中加入bin的路径。

## 写作提示

-  参看示例模板 `main.tex` 或 `example.tex` 及其中插入的各章节 `tex/*.tex` 或 `example_tex/*.tex` 熟悉模板结构和 $LaTeX$ 语法，撰写论文正文。
-  在写公式时，请不要在公式之后加入额外的空行，避免空行所导致的公式与下一行距离过大的问题。
-  在编译时，请使用xelatex进行编译。
-  在写参考文献时，可以先选用GBT7714-2015.bst来查看缺少哪些关键内容，进行补全，如果存在某些内容找不到的问题，则可以使用GBT7714-2015-NoWarning.bst来不表示这些缺乏信息。
-  在写表时，如果存在上下两个线加粗的需求，可以使用\toprule[], \midrule[] 和 \bottomrule[] 来加粗三线表的三条线。
-  在写论文时，可根据tex文件里的注释信息来修改本文的密级，专硕学硕等内容。
-  在编译时，可能会出现参考文献无法出现的现象，此时，可以先运行texstudio界面上方工具栏的参考文献，然后进行重新的构建和编译，即可出现参考文献内容。
-  在编译时，有可能会出现两行间距过小的情况，这是由于本页的图的大小导致的，当遇到这种情况时，可在间距较小的第二行之前加入\newpage使其进入下一页，可解决这个问题。
