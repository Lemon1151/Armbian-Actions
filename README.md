- stable：kernel-6.1；current：kernel-6.6；edge：kernel-最新

# 仓库说明 
- rk3399-test分支是测试分支，主要用来验证dts/patch的可行性
- rockchip64-current存放current（rockchip64-6.6）,edge（目前是rockchip64-6.11）的patch/dts文件通过软链接让一份文件实现复用
- rockchip64-6.1存放stable（自定义内核分支，armbian没有这个分支，默认为current-6.6）
- stable必须要在xxx.conf的KERNEL_TARGET选项添加stable

# Armbian-Actions  
- 通过GitHub Actions构建armbian支持列表之外的rk33xx设备固件
- 此仓库仅提供armbian构建方法、思路；如出现固件不能用、外设不能用等等问题请自行寻找解决方法
- Armbian branch的stable选项必须要构建的板卡支持这两个分支才选择，否则会报错
- Armbian kernel是Armbian构建过程中自动编译生成的产物
- Armbian源码https://github.com/armbian/build

## Links  
- [armbian](https://github.com/armbian/build)
- [ophub](https://github.com/ophub/amlogic-s9xxx-armbian)
- [cm9vdA](https://github.com/cm9vdA/build-armbian)
- [Lollipop907](https://github.com/Lollipop907)
- [xiaomeng9597](https://github.com/xiaomeng9597/iStoreOS-For-RK33XX)
- [QXY716](https://github.com/QXY716/Fine3399-rk3399-armbian)
