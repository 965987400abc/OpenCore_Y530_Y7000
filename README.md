# OpenCore_Y530_Y7000
# Y7000-Y530_OpenCore适用于macOS 10.15.2\10.14.6\10.13.6
# 重申OpenCore的重要事项：不要使用Configurator进行config.plist配置，该工具会破config.plist的文件结构，建议使用Xcode 或者ProperTree。
# Y7000 2018款bios设置：FN+D+O进入
# 关闭如下：
# UART0	ICONG2c	Advanced>PCH-IO>serallo Configutatin>UART0
# 打开如下：
# EHCI/XHCI Hand-off	 EHCI/XHCI 	Advanced>USB Configutatin>Usb Legacy SMI
# Debug serial 	串行端口	Advanced>Debug settings>改为：legacy URAT
# 以上设置不会影响到Windows的使用！
# A:升级Catalina分两种：
# 1.单独硬盘安装的mac 可直接升级，我是特地从新安装10.14.6开始测试，一直升级到10.15.1再到10.15.2，没有问题，但我不保证在您的设备上会顺利，注意备份   好重要资料；
# 2.Windows和MAC共存的磁盘，不建议直接在线升级，中午帮群友装了一台，翻车了，最后还是全新安装才搞好！
# B:升级模式和全新安装
# 单硬盘在线升级：替换EFI，在WINDOWS用DG替换，在OC引导界面清除NVRAM后再进入系统，下载升级！
# 全新安装：替换EFI后直接引导即可：
  
