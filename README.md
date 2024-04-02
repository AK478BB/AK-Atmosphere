# AK原版大气层1.7.0个人整合包（2024.4.2）

【00—此次版本更新的特别说明】

（1）和0314版相比，0402版更更新atmosphere-1.7.0-prerelease-35d93a7c4，hekate_ctcaer_6.1.1_Nyx_1.6.1，Sigpatch，最高支持SW18.0.0系统。更新MissionControl-0.11.0-master-2f5e9b9，ldn_mitm--v18.0，Lockpick_RCM--v1.9.12，如当前正在用AK原版大气层1.5.5（1002版）或以后的个人整合包的，且没加过其它插件的，直接覆盖新版AK大气层整合包。

由于atmosphere-1.7.0开始，作者删除KIP的功能会影响FS补丁的加载，极限超频的loader.kip等一系列问题。也就是sigpatch签名补丁失效，不能玩破解游戏，但是这仅限于fusee引导（大气层-自动识别），所以atmosphere/kip_patches可有可无。通过Hekate的fss0引导的真实（破解）系统，虚拟（破解）系统的KIP是通过bootloader/patches.ini实现，所以不受大气层1.7.0升级导致不能玩破解游戏的影响。

AK_ATM_1.7.0_0402.7z是AK原版大气层1.7.0个人整合包0402版

<img src="https://github.com/AK478BB/AK-Atmosphere/raw/branch/main/AK_ATM_1.5.1_0329.jpg">
