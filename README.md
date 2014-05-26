### Sublime Text Imfix

This repo is aimed to do three things:

+ Install Sublime Text 3
+ Install Fcitx Input Method
+ Fix Sublime Text 2/3's input method problem under Ubuntu(Debian) System

### Step to use this repo ###

+ Update and then upgrade your system to the newest

```bash
sudo apt-get update && sudo apt-get upgrade
```

+ Clone this repo in your local directory : 

```bash
git clone https://github.com/lyfeyaj/sublime-text-imfix.git
```
    
+ Change your current directory to this folder `sublime-text-imfix`:

```bash
cd sublime-text-imfix
```
    
+ Run the below script : 

```bash
./sublime-imfix
```

+ Done! Re-login your X windows. And then you can enjoy using Sublime Text 3 with Fctix Input Method!

### Completion Preview Image:

![Fcitx](image/fcitx.png)

### Important Note

+ **Sublime Text 3 input method fix only works when calling from terminal, such as `subl .`**

### Todo

+ Add compile detail to this README

```bash
gcc -shared -o libsublime-imfix.so sublime_imfix.c  `pkg-config --libs --cflags gtk+-2.0` -fPIC
```

--------------

### Sublime Text 2/3 输入法修复[Ubuntu(Debian)]

主要目的:

+ 安装 Sublime Text 3
+ 安装 Fcitx 输入法 + 皮肤
+ 修复 Sublime Text 2/3's 在 Ubuntu(Debian) 系统下的无法输入中文输入法的问题

### 使用方法 ###

+ 更新并升级系统为最新(较新的系统会解决很多可能出现的问题)

```bash
sudo apt-get update && sudo apt-get upgrade
```

+ 克隆项目到本地 : 

```bash
git clone https://github.com/lyfeyaj/sublime-text-imfix.git
```

+ 运行脚本 : 

```bash
cd sublime-text-imfix && ./sublime-imfix
```

+ 完成! 重新启动后就可以在Sublime Text 2/3 中 使用Fcitx了!

### 效果图:

![Fcitx](image/fcitx.png)

### 重要提示:

+ **这个修复仅当在终端中使用 `subl .` 调用Sublime Text的时候有效, 具体原因请看源代码[src/subl](https://github.com/lyfeyaj/sublime-text-imfix/blob/master/src/subl)**
