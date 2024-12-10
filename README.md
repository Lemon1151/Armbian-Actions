
# 简介
- 通过GitHub Actions构建armbian支持列表之外的rk35xx设备固件
- 此仓库仅提供armbian构建方法、思路；如出现固件不能用、外设不能用等等问题请自行寻找解决方法
- Armbian branch的stable选项必须要构建的板卡支持这两个分支才选择，否则会报错
- Armbian kernel：linux-dtb、linux-headers、linux-image、linux-libc-dev四个deb包
- Armbian源码https://github.com/armbian/build

## 仓库详情
- rk35xx-legacy存放legacy（5.10）,rk35xx-vendor-6.1存放vendor（6.1）的patch/dts文件
- archive/rockchip-rk3588-6.12(目前6.12)存放最新内核patch/dts文件
- legacy,vendor,edge,current必须要xxx.conf的KERNEL_TARGET选项支持

## yml工作流文件说明  
- build armbian all borad.yml：构建列表内所有设备armbian固件，不上传kernel headers文件
- build armbian customize board.yml：单独构建某设备armbian固件，不上传kernel headers文件
- build armbian kernel customize.yml：单独构建某设备armbian固件，将headers、image、dtb、libc-dev上传至[Armbian Kernel](https://github.com/Lemon1151/Armbian-Actions/releases/tag/Armbian_Kernel)标签
- build kernel customize.yml：单独构建，只上传headers、image、dtb、libc-dev至[Armbian Kernel](https://github.com/Lemon1151/Armbian-Actions/releases/tag/Armbian_Kernel)标签

## Links  
- [armbian](https://github.com/armbian/build)
- [ophub](https://github.com/ophub/amlogic-s9xxx-armbian)
- [cm9vdA](https://github.com/cm9vdA/build-armbian)
- [Lollipop907](https://github.com/Lollipop907)
- [xiaomeng9597](https://github.com/xiaomeng9597/iStoreOS-For-RK33XX)
- [QXY716](https://github.com/QXY716/Fine3399-rk3399-armbian)
