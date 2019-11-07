# openwrt18.06

1. 首先装好 Ubuntu 64bit

2. 命令行输入 sudo apt-get update ，然后输入
sudo apt-get -y install build-essential asciidoc binutils bzip2 gawk gettext git libncurses5-dev libz-dev patch unzip zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs git-core gcc-multilib p7zip p7zip-full msmtp libssl-dev texinfo libglib2.0-dev xmlto qemu-utils upx libelf-dev autoconf automake libtool autopoint device-tree-compiler

3. git clone https://github.com/Ameykyl/openwrt18.06-1 命令下载好源代码，然后 cd openwrt18.06-1 进入目录

4. ./scripts/feeds update -a 
   ./scripts/feeds install -a
   make menuconfig 

5. 选好你要的路由，输入 make -j1 V=s （-j1 后面是线程数）即可开始编译你要的固件了。
