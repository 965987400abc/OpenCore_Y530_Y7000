
## Y7000-Y530_OpenCore适用于macOS 10.15.2\10.14.6\10.13.6

## Y7000 2018款高级bios设置：FN+D+O进入
- 按F9恢复默认bios设置，仅需要修改以下设置：
- Advanced>Debug settings>legacy URAT
## 注意事项
- config.plist里面的三码已删除，请自行使用Clover Configurator算出三码；

## 模拟NVRAM方法：
- 将LogoutHook文件夹放到文档路径，在终端输入：
- sudo defaults write com.apple.loginwindow LogoutHook /Users/你的用户名/Documents/LogoutHook/LogoutHook.command
- 终端会提示输入密码，密码打进去不显示（正常现象）；
- 重启后，你会在/EFI/下看到nvram.plist，代表已经成功模拟了；

## 设置默认启动项
- 模拟nvram成功后，在系统设置选择默认启动的OS即可；

## 欢迎各位机友加入Q群探讨完善
- 857996987 （OpenCore Y7000）
