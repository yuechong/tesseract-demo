# tesseract-demo
windows


第一步：下载安装包

https://github.com/UB-Mannheim/tesseract/wik


第二步：安装

http://ourcodeworld.com/articles/read/348/getting-started-with-optical-character-recognition-ocr-with-tesseract-in-node-js

第三步：配置环境变量

注意：我的系统是win7，其他系统应该差不多，跟配置java变量一样

复制你的安装地址，我的是安装在C:\Program Files (x86)\Tesseract-OCR，



复制安装路径“C:\Program Files (x86)\Tesseract-OCR”，


配置环境变量：



把刚才的安装路径“C:\Program Files (x86)\Tesseract-OCR”添加PATH和Path，注意，添加时候开头用“;”跟之前的变量隔开，结尾以“;”结尾。下面是我的配置信息样本：

C:\Program Files (x86)\Tesseract-OCR;

配置好了点击保存。

 

打开命令终端，输入：tesseract -v，可以看到版本信息



如果出现报错，估计是环境变量没配置好。

到这里，我们就算安装完成了，但是，我们的系统还是无法识别中文的，我们要去下载简体汉字、繁体汉字语言包（上文给了地址了），下载好之后放到安装目录的tessconfigs目录下即可。

补充：因为没有配置全局变量，无法跨盘执行数据转换，这里我们在环境变量那增加一个配置信息

系统变量—->新建：

增加一个TESSDATA_PREFIX变量名，变量值还是我的安装路径C:\Program Files (x86)\Tesseract-OCR;
