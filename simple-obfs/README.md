tar xjf openwrt-sdk-21.02-bcm27xx-bcm2711_gcc-8.4.0_musl.Linux-x86_64.tar.bz2
cd openwrt-sdk-*
git clone https://github.com/shadowsocks/openwrt-feeds.git package/feeds
git clone https://github.com/aa65535/openwrt-simple-obfs.git package/simple-obfs
make menuconfig
make package/simple-obfs/compile V=99
