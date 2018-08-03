git clone https://github.com/friendlyarm/kernel-rockchip --depth 1 -b nanopi4-linux-v4.4.y
cd kernel-rockchip
make ARCH=arm64 nanopi4_linux_defconfig
make ARCH=arm64 nanopi4-images

change cross compile prefix to your compile in nanopi4_linux_defconfig.
Config cross compile environment.
