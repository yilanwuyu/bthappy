感恩loc的大佬提供了方法，只是把方法放进了脚本里，
在Centos上默认安装路径测试成功。
大佬提供的安装脚本，保存了一下。
curl -sSO https://raw.githubusercontent.com/yilanwuyu/bthappy/main/iinstall_panel.sh && bash install_panel.sh
宝塔7.7开心脚本，命令集成在了脚本里，但是！这里是用我修改好的plugin和repair的文件进行替换，介意误用。
curl -sSO https://raw.githubusercontent.com/yilanwuyu/bthappy/main/one_key_happy.sh && bash one_key_happy.sh
挂载硬盘
yum install wget -y && wget -O auto_disk.sh https://raw.githubusercontent.com/yilanwuyu/bthappy/main/auto_disk.sh && bash auto_disk.sh

由于本人过于菜鸡，先安装脚本安装好之后运行开心脚本，然后再挂载硬盘，无多硬盘忽略就行。因为文件路径写死了/www/server/panel/data
开心的脚本内容都是可读的。
也可以使用https://cdn.jsdelivr.net/gh/ztkink/bthappy@main/进行替换。
建议自存plugin和repair文件，然后替换one_key_happy.sh的地址。


操作方法
记得先切到 root 用户下进行操作

下载 7.7.0 版本更新包

wget https://github.com/yilanwuyu/bthappy/releases/download/7.7.0/LinuxPanel-7.7.0.zip
解压

unzip LinuxPanel-7.7.0.zip
压缩包应该会解压得到一个 panel 文件夹，如果不是的话，说明你下载的包不对。

进入文件夹

cd panel/
运行更新脚本降级

bash update.sh
更新脚本执行的覆盖操作，所以可以用来降级。

开启离线模式

前往“面板设置”页面，在上面开启“离线模式”，这样可以防止面板自动更新（不知道宝塔会不会有强制更新，如果有那也太过分了吧） 
作者：ChrisKim_ZHT https://www.bilibili.com/read/cv17006523 出处：bilibili
