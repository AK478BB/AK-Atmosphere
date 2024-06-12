# AK原版大气层1.7.1个人整合包（2024.6.13）

（1）和0603版相比，0613版更新Atmosphere1.7.1，Hekate6.2.0汉化，Sigpatch，最高支持switch18.1.0系统，更新ovlEdiZon--v1.0.8，MissionControl-0.11.1，ldn_mitm--v18.1.0，FPSLocker锁帧补丁，18.1.0系统主题所需的systemPatches补丁。更新极限超频EOS1.3.0。

因为是原版atmosphere，所以大气层-自动识别fusee引导不支持sigpatch，不能玩破解游戏，可以等大佬编译大气层1.7.1内置sigpatch后再替换，暂时屏蔽Fusee引导的启动项。

AK_ATM_1.7.1_0613.7z是AK原版大气层1.7.1个人整合包0613版

AK从0425版开始，对整合包内容进行分类

00基本包--AK大气层1.7.1无Tesla整合版

内容：大气层三件套基本组件+相册NRO插件（有金手指edizon.nro插件），可独立使用，满足标准需求。

01叠加包--AK原版Tesla插件包

内容：原版Tesla核心组件+金手指+超频+底座+蓝牙手柄+锁帧+模拟Amiibo+联网等插件

02替换包--AK极限超频插件

内容：极限超频插件EOS，支持最新SW系统。

（2）升级说明

如果首次想替换成无Tesla版的00基本包，需要保留nintendo和emummc后删除其它，再覆盖00基本包，以后更新是可以覆盖升级。

如果这次更新是想继续使用Tesla插件（和AK上一版的大气层一样）请先覆盖00基本包，再覆盖01叠加包。

00基本包是必须的，因为没有Tesla插件和sysmodule启动器，所以无Tesla版的大气层整合包非常稳定，玩游戏不会报错，如果你连主题也不安装，系统会更加稳定，无Tesla插件的大气层整合包等同大气层纯净包。

01叠加包是可用可不用，可以覆盖到00基本包，也可以给其它类似的大气层三件套纯净包使用，除了Tesla-Menu外，为避免冲突，其余插件禁止自启动，启动其它sysmodule，第一次要去Deepsea工具箱启动。

02替换包只能替换到01的Tesla插件包中且是给AK大气层整合包使用，替换里面的普通超频插件，只建议续航和OLED极限超频，并不推荐非续航和Lite极限超频，极限超频有损坏硬件不可逆的风险。

00基本包和01叠加包之间有两个文件重叠：edizon.nro和DeepSeaToolbox.nro

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/AK_ATM_1.5.1_0329.jpg">
