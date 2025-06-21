# AK原版大气层1.9.1个人整合包（2025.06.21）

（1.4）20250621版更新NXThemesInstaller--v2.8.1和20.1.5系统需要systemPatches补丁，更新ultrahand--v1.9.5，ovlEdiZon--v1.0.10，SaltyNX--v1.3.0pre6，FPSLocker.ovl--v2.2.0pre5和FPSLocker锁帧补丁，更新EOS-OC-Suite--v1.6.2.2，loader.kip不变。

（1.3）20250615版更新zdm大佬最新atmosphere-1.9.1，在system_settings.ini中加一条参数add_nintendo_blocking_to_dns_hosts = u8!0x0，可以删除atmosphere/hosts/sysmmc.txt和显示真实系统序列号，解决真实（破解）系统联机问题，更新nx-ovlloader--v1.1.1+，ultrahand--v1.9.2，ovlSysmodules--v1.3.4，Status-Monitor-Overlay--v1.1.9+r3，sys-con--v1.5.4，更新FPSLocker锁帧补丁，更新极限超频EOS-OC-Suite--v1.6.2，更新Goldleaf--v1.1.1，Tinfoil--v20.0v1。

（1.2）20250607版更新zdm大佬发布的内置签名补丁的atmosphere-1.9.1-master-with sigpatch，CommonProblemResolver--v0.3.4，更新Tesla-ultrahand--v1.8.9，sys-con--v1.5.3，SaltyNX--v1.3.0pre4，FPSLocker.ovl--v2.2.0pre3和FPSLocker锁帧补丁，更新极限超频EOS-OC-Suite--v1.6.1支持大气层1.9.1。

（1.1）20250530版更新zdm大佬发布的内置签名补丁的atmosphere-1.9.1-master-with sigpatch，hekate_ctcaer_6.3.1_Nyx_1.7.0，Sigpatches for Atmosphere 1.9.1，更新Tesla-ultrahand--v1.8.5，Status-Monitor-Overlay--v1.1.9+，MissionControl-0.13.2，ldn_mitm--v1.19.1，SaltyNX--v1.2.7，FPSLocker.ovl--v2.1.5和FPSLocker锁帧补丁。更新20.1.1的主题ips补丁，nxdumptool.nro。

# 【AK杂谈】巧用带转区的Tesla系统模块实现国行20.0.1系统救砖

感谢cccvivi的贴国行20.01救活了！AK大，昨天一直看你的贴子吓死我了，可以不用线刷修复强刷20.0.1的国行真实系统了

https://www.tekqart.com/thread-420905-1-1.html

感谢zdm65477730大佬编译的Tesla终极版套件，只需要Tesla基础的三件套就行了。

Tesla插件列表

（1）-（3）是特斯拉核心组件，也叫特斯拉基础包

（1）nx-ovlloader，Tesla启动器

https://github.com/zdm65477730/nx-ovlloader/releases

（2）ovlmenu，Tesla菜单

https://github.com/zdm65477730/Tesla-Menu/releases

（3）ovlSysmodules，Tesla系统管理

https://github.com/zdm65477730/ovl-sysmodules/releases

对于国行系统强刷20.0.1导致的2162-0002变砖出错，可以通过zdm65477730大佬编译的Tesla终极版套件中的带转区功能的系统模组“ovl-sysmodules.ovl“，实现在出现Switch图标的时候快速打开Tesla菜单，进入系统模组，按Y键实现实时转区。因为时间很短，只有一两秒，所以不仅要手速，而且还要设置Tesla插件的快捷键，让ovlmenu只能显示系统模组ovl-sysmodule，而且要屏蔽ovl-sysmodules里除了转区之外的其它功能。

AK进行了实验，需要做纯净的tesla三件套，ovlloader，ovlmenu和ovlsysmodules , Tesla快捷键设定L，ovlsysmodules里面只能显示转区功能。

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/tesla%E6%95%91%E5%9B%BD%E8%A1%8C20.0.1.jpg?raw=true" align="center" width="100%" />

# 操作方法：开机进破解系统，在出现大气层三角形图标后拼命按L，一旦出现tesla菜单的系统模块，马上按A，然后按Y切换到国际，这样就能顺利进入系统了。如果失败了重启再进入。

<img src="https://github.com/AK478BB/ATM-Instruction/blob/main/%E6%89%8B%E6%8A%8A%E6%89%8B%E6%95%99%E4%BD%A0%E7%AE%A1%E7%90%86%E5%A4%A7%E6%B0%94%E5%B1%82tesla%E5%92%8Covl%E6%8F%92%E4%BB%B6.jpg?raw=true" align="center" width="80%" />

# 【AK杂谈】SW国行系统不可强刷20.0以上，会有2162-0002变砖出错

因为考虑到国行Switch1肯定永久停留在19.0.1，那么AK想到很多小伙伴的国行硬破的虚拟系统可能直接使用国行系统，以后等大气层三件套更新适配也可以通过daybreak离线升级到20.0.0+的系统，考虑到国行系统离线升级强刷可能存在的问题，AK特地测试了国行虚拟系统。
结果很悲催：新做好的19.0.1虚拟系统转成国行系统后，daybreak升级20.0.1

出错代码：2162-0002（0x4a2）

程序：0100000000001000

系统固件：20.0.1（大气层1.9.0）

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/2162-0002.jpg?raw=true" align="center" width="80%" />

但是同样全球系统19.0.1，daybreak升级到20.0.1没问题，和两位朋友联系帮忙在非续航，国行的主机上测试，他们反馈得到了同样的结果。假如是全球系统20.0.0或20.0.1，通过相册插件tencent-switcher-gui.nro改成“国行系统”以后重启，一样卡在这个错误无法解决。

因为测试是在虚拟系统，而且还是文件格式的SD01，所以测试后，他们可以把这个SD01的虚拟系统删除，对主机没有任何的影响，也不影响他们SD00里的虚拟系统。

AK提醒：所有国行Switch破解双系统的小伙伴们，请尽快把你国行主机上的虚拟系统，从“国行系统”改“全球系统”，相册里有插件tencent-switcher-gui.nro，一键切换虚拟系统变成全球系统，不要尝试daybreak升级国行的虚拟系统到20.0.0或以上，等切换变成全球系统以后才可以daybreak升级。

如果是单系统破解的小伙伴，想必已经是BAN机了吧，要么做个虚拟系统，要么把真实系统也像虚拟系统一样，改“全球系统”，然后才能升级。

# 【AK杂谈】可能Switch1的国行主机将永久停留在19.0.1系统

AK手里没有国行机，五一时遇到一位朋友玩国行正版马车8的联机，是双系统的，AK提醒有20.0.0的更新，大气层目前还未适配，但是直到全球Switch都升级20.0.1了，国行Switch1好像还是19.0.1没有推送更新，AK还以为是不是国服延迟更新，但是SW系统升级固件应该是统一分发，各区的eshop商城服务器作为节点提高升级速度，所以想想也不太可能因为国服延迟更新，AK特地去Switchbrew查了查20.0.0固件信息。

https://switchbrew.org/wiki/20.0.0

<img src="https://github.com/AK478BB/AK-Atmosphere/blob/master/CHN19.0.1.jpg?raw=true" align="center" width="80%" />

好家伙，原来Switch20.0.0的系统文件已经移除国行的相关模块，看来20.0.0系统可能因为虚拟游戏卡，分享Switch2等方面的考虑，觉得系统开发如果还要兼容Switch1国行的主机，可能也会非常麻烦，而且毫无意义，毕竟2026年5月关闭国服了。

所以国行Switch主机的正版系统可能将永久停留在19.0.1系统，熔断永远=20。但是玩国行Switch主机的小伙伴也没必要担心，因为不影响你的虚拟系统等大气层三件套全部适配后再升级20.0.1玩最新的破解游戏。
