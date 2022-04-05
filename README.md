AK原版大气层个人整合包更新须知

https://pan.baidu.com/s/1t7kvfTKvSZAOMgR6yZM3hA提取码avmd

（1）如一直用AK原版大气层个人整合包的，只要未特别说明，可以覆盖，也可以删除旧的atmosphere/contents后就覆盖新的整合包。

如原来别人的整合包上覆盖出现问题，请删除atmosphere和bootloader后再解压缩包覆盖。最稳的，请保留nintendo和emummc后删除其它，再解压缩包覆盖。

（2）软破机需要更换注入器里的payload.bin，如注入器里已经是hekate4.2或以上版本则无需更新。

短接+注入开机，点击launch，根据选择进入

cfw(sysnand)：真实系统破解状态，Hekate的FSS0引导，可以正版修改

cfw(emunand)：虚拟系统破解状态，Hekate的FSS0引导，可以破解游戏

ofw(sysnand)：真实系统不破状态，Hekate的FSS0引导，可以正版联机

cfw(auto)：大气层原版Fusee引导，根据emummc.ini自动识别真实和虚拟系统

（3）硬破机直接点击电源键开机，之后与软破机launch方式一样，补丁机与续航和lite机无差别。

使用须知

特斯拉按键： L+方向键下

启动90dns屏蔽任天堂服务

隐藏序号系统屏蔽任天堂服务

软破机和补丁机可fastcfwswitch切换系统

hbmenu.nsp装完可删

tinfoil.nro自动安装

默认tesla插件启动

除了Tesla-Menu外，为避免冲突，其余插件禁止自启动，可在deepsea toolbox中设置，设置完毕按home保存退出重启。如因自启致死机，可在电脑读取TF卡，删除atmosphere/contents/对应插件编号/flags/boot2.flag
