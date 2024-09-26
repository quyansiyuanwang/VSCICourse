# Visual Studio Code Insiders 运行C/C++程序 (安装)教程

## 注意事项

* 以下简称
  * `Visual Studio Code Insiders` 为 `VSCI`

* 注意
  * 在本教程中所有看到的蓝色字体都可进行点击跳转，请不要傻愣愣的看着屏幕！！！
  * 本教程建议在 `PC(电脑)端` 进行查看，手机端可能会操作不便！
  * 本教程仅供学习使用，不得用于商业用途！
  * 本教程仅比较完美的适配 `Windows系统用户` 使用！

## 目录

1. [下载](#下载教程)
2. [安装](#安装教程)
3. [配置](#配置教程)
4. [使用](#使用教程)

## 教程

### 下载教程

1. 下载必备的 `VSCI`, `msvc`  
    [不懂如何下载？](/Download.MD)
2. 下载完毕后, 找到下载文件所在位置  
    [找不到文件位置？](/Download.MD/#文件位置)

### 安装教程

1. 解压缩 `msvc压缩包` 和 `VSCI压缩包`  
    [如何解压缩](/Unzip.MD)
2. 将解压文件放到你想放的位置，我个人放U盘随身携带  
    [不知道放哪？](/Hopeless.MD)  
    [什么是U盘？](/Hopeless.MD)

### 配置教程

1. 打开 `VSCI` 的根目录，如图所示  
    ![打开VSCI根目录](/images/VSCInsidersConfig/1.png)
2. 在你 `VSCI` 的根目录下新建文件夹 `data`  
    [不知道如何新建文件夹？](/Hopeless.MD)  
    [什么是根目录](/Crap.MD)
3. 鼠标左键双击运行 `VSCI` 根目录下的 `Code - Insiders.exe` 如下图所示  
    ![VSCIExe](/images/VSCInsidersConfig/2.png)
4. 运行 `VSCI` 后如图所示, 点击左侧的 `扩展` 图标  
    ![VSCIUI](/images/VSCInsidersConfig/3.png)
5. 在左上侧的搜索框搜索 `C/C++` 
    ![VSCISearchExtensions](/images/VSCInsidersConfig/4.png)
6. 点击如下 `install` 按钮安装 `C/C++` `C/C++ Runner` 和 `C/C++ Extension Pack` 扩展  
    ![VSCIInstallExtensions](/images/VSCInsidersConfig/5.png)
7. 请耐心等待安装完毕
8. 如出现 `restart Extension` 按钮，请点击并耐心等待，必要时重启 `VSCI`(必要时 `VSCI` 会提醒你重启)
9. 安装完毕后，点击左上角的 `文件` 图标  
    ![JumpFilePage](/images/VSCInsidersConfig/6.png)
10. 跳转到 `文件` 页面后，点击 `Open Folder` 按钮打开文件夹，如下图所示点击  
    ![ClickOpenFoleder](/images/VSCInsidersConfig/7.png)
11. 选中或打开一个想打开的文件夹后点击 `选择文件夹` ，如我个人下图所示  
    ![OpenFolder](/images/VSCInsidersConfig/8.png)
12. 起初文件夹下没有任何内容，如图  
    ![UnderFolder](/images/VSCInsidersConfig/9.png)
13. 我们创建一个新的代码工程文件，例如 `main.c` ，如图  
    ![ClickCreateFile](/images/VSCInsidersConfig/10.png)
    ![CreateFile](/images/VSCInsidersConfig/11.png)
14. 点击其他空白处或按下 `Enter` 键完成创建后，如图所示出现了两个东西，一个是 `.vscode` 工程配置文件夹，一个是 `main.c` 代码文件  
    ![AfterCreating](/images/VSCInsidersConfig/12.png)
15. 现在我们按图示顺序依次点击，打开 `.vscode` 文件夹下的 `c_cpp_properties.json` 的json文件  
    ![OpenConfigJson](/images/VSCInsidersConfig/13.png)
16. 可以看见一行有 `"compilerPath": "D:/CodingCompiler/mingw32/bin/gcc.exe",`，如图  
    ![SeeCompilerPath](/images/VSCInsidersConfig/14.png)
17. 打开你解压后的 `msvc` 编译器文件目录，如图  
    ![msvcFileRoot](/images/VSCInsidersConfig/15.png)
18. 一路点开 `\mingw32\bin` 目录，来到 `bin` 文件目录，如图  
    ![OpenBin](/images/VSCInsidersConfig/16.png)
19. 点击上方导航栏，复制当前 `bin文件夹` 的路径，如图  
    ![CopyPath](/images/VSCInsidersConfig/17.png)
20. 将其复制到刚刚json文件中那行冒号后双引号内，注意逗号与双引号不要丢！如图  
    ![PastePath](/images/VSCInsidersConfig/18.png)
21. 由于是 `Windows系统` 所以路径由 `\` 分割，而在json语言中在每个 `\` 后都会被转义，所以我们要把这些单`\`写成`\\`或`/`，如图  
    ![ConvertPath](/images/VSCInsidersConfig/19.png)
22. 我们再在 `bin` 的后面添加上 `\\gcc.exe` 或 `/gcc.exe`，如图  
    ![AddGcc](/images/VSCInsidersConfig/20.png)
23. 随后点击 `x` 再点击 `Save` 关闭json文件，如图  
    ![CloseJson](/images/VSCInsidersConfig/21.png)  
    ![SaveJson](/images/VSCInsidersConfig/22.png)

### 使用教程

现在你就可以打开 `.c` 文件，然后点击右上角的小三角图标进行编译并运行啦，如图  
![Run](/images/RunC.png)
