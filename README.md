AK原版大气层1.6.2个人整合包（2023.12.28）

更新须知

（1）如当前正在用AK原版大气层1.5.5（1002版）或以后的个人整合包的，且没加过其它插件的，直接覆盖新版AK大气层整合包

如果加过插件，也可以删除内存卡上旧的atmosphere/contents，config，switch/.overlays和saltysd四个目录后覆盖新的AK大气层整合包。

如原来别人的整合包上覆盖出现问题，最稳的，请保留nintendo和emummc后删除其它，再解压缩包覆盖。

（2）不区分软破和硬破机，软破是短接+注入开机，TX注入器直接用，大气层注入器替换内置Payload.bin，整合包根目录是最新的Hekate重命名的payload.bin，如注入器内置hekate4.2或以上则无需替换。硬破是直接点开机键开机，之后与软破无差别。

点击launch，根据选择进入

cfw(sysnand)：真实系统破解状态，Hekate的FSS0引导，可以正版修改

cfw(emunand)：虚拟系统破解状态，Hekate的FSS0引导，可以破解游戏

ofw(sysnand)：真实系统不破状态，Hekate的FSS0引导，可以正版联机

cfw(auto)：大气层原版Fusee引导，根据emummc.ini自动识别真实和虚拟系统

点击more configs，根据选择进入

Lakka-Erista，是AK大气层原来设定的旧lakka模拟器。它只支持软破或补丁机，但能兼容exfat格式的sd卡

Lakka-l4t：是新的lakka模拟器，兼容mariko/oled，目前新lakka只能支持fat32格式的sd卡

ubuntu-l4t：是新的ubuntu系统，兼容mariko/oled，目前新ubuntu只能支持fat32格式的sd卡

lockpick_rcm：主机Keys提取软件

CommonProblemResolver：主机启动修复软件

TegraExplorer：主机文件管理软件

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/AK_ATM_1.5.1_0329.jpg?raw=true" align="center" width="80%" />
