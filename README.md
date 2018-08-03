# Source
git clone https://github.com/friendlyarm/kernel-rockchip --depth 1 -b nanopi4-linux-v4.4.y

# Compile
cd kernel-rockchip
make ARCH=arm64 nanopi4_linux_defconfig
make ARCH=arm64 nanopi4-images

## Note
change cross compile prefix to your compile in nanopi4_linux_defconfig.
Config cross compile environment.

# Update kernel for Ubuntu
After compile, kernel.img and resource.img will be generated.
Update these two images by Linux_Upgrade_Tool_1.27.rar which can be found in [tools](https://pan.baidu.com/s/1rZmMQEQL1tu15R6IeYrksw#list/path=%2FFriendlyELEC-RK3399%2Ftools)
