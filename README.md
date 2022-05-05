# WDControl
Windows Defender 状态设置工具


在一次系统封装时，之前用的离线添加注册表“DisableAntiSpyware”的方式失效了，稍微搜了下，发现 1909 的 WD 默认启用了“篡改保护”功能，所以无法通过注册表，以及组策略关闭，只能在 WD 设置里手动关闭；Sordum 的 Defender Control 可以绕过进行关闭，但是会有一定几率造成注册表项丢失。。。。。就是这个原因，我还以为是我的 WTDR 哪里出现了问题，测试了十几遍才发现是他的问题。

那咋办嘛，自己造轮子呗，国内相关论坛逛了一遍，都是注册表，组策略，Dism++，这些方法对默认启用了“篡改保护”功能的 WD 毫无作用，最后还是在 MDL 论坛找到了 Sordum 提供的一些思路，然后摸索尝试，然后就有了这个，不用破坏文件，不影响其他功能，无副作用，并且可以反禁用的小工具~

功能
禁用 Windows Defender
启用 Windows Defender
移除 Windows Defender
命令行说明
/Disable        禁用 Windows Defender
/Enable         启用 Windows Defender
/KillWD        移除 Windows Defender
移除 Windows Defender 也不会有任何提示的，请谨慎执行

截图




禁用WD后请及时安装第三方杀软确保计算机安全！