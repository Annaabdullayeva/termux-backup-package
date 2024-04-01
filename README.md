个人制作的打包好的各种termux数据包，一键导入使用，使用前请先看readme

该项目中所有懒人包均利用以下指令制作：

tar -zcf /sdcard/备份.tar.gz -C /data/data/com.termux/files ./home ./usr

使用方法：

将你需要的懒人包名字改为“备份.tar.gz”后放在手机sd卡根目录（就是你点开手机文件管理的那个目录），然后执行以下指令。

tar -zxf /sdcard/备份.tar.gz -C /data/data/com.termux/files --recursive-unlink --preserve-permissions

以下是各个包的说明（更新中）：

1.自带xfce、firefox：

安装好了xfce桌面（直接装在termux里的，不是容器）和Firefox浏览器，可以安装好termux及termux x11后直接用以下命令启动图形化界面：

termux-x11 :0 -xstartup "dbus-launch --exit-with-session xfce4-session"

2.mobox

提前配置好了mobox容器的包，在termux中输入mobox，选择第一项，按ok即可启动，内部是一个类Windows环境，可以运行一些Windows软件

（更新中）
