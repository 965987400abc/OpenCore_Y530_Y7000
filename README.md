# OpenCore_Y530_Y7000
Y7000-Y530_OpenCore适用于macOS Mojave10.14.6-10.13.6
//
前言：
    重申OpenCore的重要事项：不要使用OpenCore Configurator进行config.plist配置，该工具会破坏config.plist文件结构，建议使用Xcode 或者ProperTree。
//
OpenCore官方要求的BIOS设置，抄袭自@黑果小兵
关闭如下：
Fast Boot	快速启动
CFG Lock (MSR 0xE2 write protection)	CFG 锁 (MSR 0xE2 写入保护)
VT-d	VT-d
CSM	兼容性支持模块
开启如下：
VT-x	VT-x
Above 4G decoding	大于 4G 地址空间解码
Hyper Threading	处理器超线程
Execute Disable Bit	执行禁止位
EHCI/XHCI Hand-off	接手 EHCI/XHCI 控制
OS type: other types	操作系统类型: 其他
以上要求个人没有按照此设置，只关闭了安全启动，就直接安装了，没什么影响，不嫌麻烦的可以按以上要求。
//
1：OpenCore文件结构，针对小白的讲解各个.efi与.KEXT文件的作用：
