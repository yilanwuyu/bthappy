感恩loc的大佬提供了方法，只是把方法放进了脚本里，
在Centos上默认安装路径测试成功。
大佬提供的安装脚本，保存了一下。
curl -sSO https://raw.githubusercontent.com/ztkink/bthappy/main/iinstall_panel.sh && bash install_panel.sh
宝塔7.7开心脚本，命令集成在了脚本里，但是！这里是用我修改好的plugin和repair的文件进行替换，介意误用。
curl -sSO https://raw.githubusercontent.com/ztkink/bthappy/main/one_key_happy.sh && bash one_key_happy.sh
挂载硬盘
yum install wget -y && wget -O auto_disk.sh https://raw.githubusercontent.com/ztkink/bthappy/main/auto_disk.sh && bash auto_disk.sh

由于本人过于菜鸡，先安装脚本安装好之后运行开心脚本，然后再挂载硬盘，无多硬盘忽略就行。因为文件路径写死了/www/server/panel/data
开心的脚本内容都是可读的。
也可以使用https://cdn.jsdelivr.net/gh/ztkink/bthappy@main/进行替换。
建议自存plugin和repair文件，然后替换one_key_happy.sh的地址。
