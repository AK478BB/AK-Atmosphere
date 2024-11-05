# AK原版大气层1.8.0个人整合包（2024.11.5）

【00—此次版本更新的特别说明】

（1）和AK原版大气层1.7.1相比。

（1.7）1105版更新Status-Monitor-Overlay--v1.1.5+，SaltyNX--v1.0.2，linkalho--v2.0.1-2a980d69，NX-Activity-Log--v1.5.0-hos19.0.0，nxdumptool--v2.0-c1b76fb-11.3.2024，更新FPSLocker锁帧补丁。

（1.6）1103版更新ultrahand--v1.8.1，SaltyNX--v1.0.0、ReverseNX-Tool.nro--v3.2.0，更新FPSLocker锁帧补丁。

（1.5）1028版更新ultrahand--v1.8.0，Status-Monitor-Overlay--v1.1.4+，SaltyNX--v0.10.0，wiliwili--v1.5.0，更新FPSLocker锁帧补丁。

（1.4）1021版更新大气层1.8.0三件套第五版（大气层三件套中的sigpatch新增nim patch补丁，功能见【AK杂谈】手把手教你了解大气层sigpatch签名补丁），更新ultrahand--v1.7.9，sys-con--v1.4.3-0682ed5，替换普通超频为EOS1.5.0，改02替换包为普通超频变极限超频的loader.kip和hekate_ipl.ini。

（1.3）1019版更新nx-ovlloader--v1.0.9+，MissionControl-0.12.0，sys-con--v1.4.2，ldn_mitm--v1.18.0，至此整合包里自带的sysmodule启动插件全部支持19.0.0系统。更新FPSLocker锁帧补丁。

（1.2）1016版更新atmosphere-1.8.0-prerelease-c6014b533，更新此版大气层的loader patch（同时支持fusee引导的ips和fss0引导的patches.ini），fusee.bin（gbatemp论坛编译版，支持fusee引导的fs/loader的ips补丁），更新FPSLocker锁帧补丁。更新极限超频EOS-OC-Suite--v1.5.0，支持19.0.0系统。

（1.1）1015版更新lsp199308编译的atmosphere-1.8.0-prerelease-5717ea6c0，hekate_ctcaer_6.2.2_Nyx_1.6.4，最高支持19.0.0系统，从此版本开始：ultrahand同名平替了Tesla组件（nx-ovlloader--v1.0.8+，ultrahand--v1.7.8，ovlSysmodules--v1.3.1+），更新ovlEdiZon--v1.0.9，Status-Monitor-Overlay--v1.1.4，SaltyNX--v0.9.4，FPSLocker.ovl--v2.0.3和FPSLocker锁帧补丁。更新19.0.0系统需要的主题systemPatches补丁，nxdumptool--v2.0-c1b76fb-10.24.2024，更新前端hbmenu.nsp，更新tinfoil.nro的applet小程序版（checkpoint.nro，dbi.nro，tinfoil.nro和wiliwili.nro都可以在安装新的hbmenu.nsp进入前端模式）。更新Lockpick_RCM--v1.9.13。

以上所有文件都是同文件名，同SD卡路径的升级，所以可相应的覆盖升级。

AK_ATM_1.8.0_1105.7z是AK原版大气层1.8.0个人整合包1105版

AK从0425版开始，对整合包内容进行分类

00基本包--AK大气层无Tesla整合版

内容：大气层三件套基本组件+相册NRO插件（有金手指edizon.nro插件），可独立使用，满足标准需求。

01叠加包--AK原版Tesla插件包

内容：Tesla核心组件（从大气层1.8.0开始ultrahand平替）+金手指+超频+底座+蓝牙手柄+锁帧+模拟Amiibo+联网等插件

02替换包--AK极限超频插件

内容：极限超频插件EOS，支持最新SW系统，非续航主机不适合极限超频。

（2）升级说明

如果首次想替换成无Tesla版的00基本包，需要保留nintendo和emummc后删除其它，再覆盖00基本包，以后更新是可以覆盖升级。

如果这次更新是想继续使用Tesla插件（和AK上一版的大气层一样）请先覆盖00基本包，再覆盖01叠加包。

00基本包是必须的，因为没有Tesla插件和sysmodule启动器，所以无Tesla版的大气层整合包非常稳定，玩游戏不会报错，如果你连主题也不安装，系统会更加稳定，无Tesla插件的大气层整合包等同大气层纯净包。

01叠加包是可用可不用，可以覆盖到00基本包，也可以给其它类似的大气层三件套纯净包使用，除了Tesla-Menu外，为避免冲突，其余插件禁止自启动，启动其它sysmodule，第一次要去Deepsea工具箱启动。

02替换包只能替换到01的Tesla插件包中且是给AK大气层整合包使用，替换里面的普通超频插件，只建议续航和OLED极限超频，并不推荐非续航和Lite极限超频，极限超频有损坏硬件不可逆的风险。

00基本包和01叠加包之间有两个文件重叠：edizon.nro和DeepSeaToolbox.nro

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/AK_ATM_1.5.1_0329.jpg">
