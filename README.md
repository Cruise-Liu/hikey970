# HiKey970开发板资料汇总
- Doc:
	- 01 hikey970烧录固件 - H-hikey(华为方案) - 深圳风火轮科技 - Powered by Discuz!.pdf
	- 02 华为HiAI DDK使用手册.pdf
	- 03 华为HiAI DDK集成手册.docx
	- 04 DevEco IDE使用指南.docx
- Bin:
	- HiAI DDK.zip: https://pan.baidu.com/s/1t3pvByq2U-tQKO1Z5fftmA
	- DevEco IDE.zip: https://pan.baidu.com/s/1IQn2tEvVA1AJTsX-4fMzSQ
	- hikey970_fix_hdmi_storage.rar(2018/05/18): https://pan.baidu.com/s/19cTv_MoIgOKgJNZJO01t4Q
- Hardware:
	- 开发板购买地址：https://item.taobao.com/item.htm?spm=a230r.1.14.16.2c705c98FLroqF&id=566806699719&ns=1&abbucket=17#detail
	- 散热风扇的安装：关键在于把正负极的插针分开，以便安装。否则由于卖家送的插针两个引脚的间距与板子的插口不匹配，导致无法安装。
	- 经过实际测试，散热风扇降温效果明显。
- Development
	- Android Studio: https://dl.google.com/dl/android/studio/install/3.1.2.0/android-studio-ide-173.4720617-windows.exe
	- SDK Manager:https://dl.google.com/android/installer_r24.4.1-windows.exe
	- JDK 8 x86-64
	- "Hello World" Project Steps:
		- a. 安装JDK、SDK Manger（安装目录不能包含空格）、Android Studio
		- b. 启动Android Studio后，在SDK Manager的位置，设置为之前安装的目录
		- c. 打开SDK Manager，下载Android SDK 26.0.2，不用设置代理，可直接下载
		- d. 新建一个hellow world项目。在编译构建时，下载gradle 4.4会耗时较长，只是慢，没有被墙
	- 注意事项：970开发板打开调制模式后，usb口的键盘和鼠标将无法使用，此时可使用蓝牙键盘鼠标代替。
	- "HiAIDemo" Project Steps:
		- a. 导入工程"Demo_Soure_Code"
		- b. 按"05 gradle-4.1-all.zip离线包下载 极速 android studio2.3 3.0编译必备 - zjgwh - 博客园",快速下载gradle-4.1-all.zip
		- c. 如图"06 hikey970 npu.png"所示，注释掉三行语句。因为无法获取到property，所以直接跳过即可
		- d. build运行到970开发板上
- 遗留问题
  - 970开发板如何使用摄像头？双目景深摄像头如何使用？
