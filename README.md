# AK大气层整合包1.7.0暂缓更新，目前有大气层1.7.0的三件套，可以直接覆盖使用，但是cfw-auto不能玩破解游戏。

【AK杂谈】大气层1.7.0后sigpatch签名补丁的三种解决办法

大气层1.7.0开始，SciresM大神删除KIP的加载功能，原来只是为了nogc卡槽保护，但是这个功能已集成在stratosphere.romfs内核中，通过stratosphere.ini调设定，不需要额外补丁。这个删除KIP的功能会影响FS补丁的加载，极限超频的loader.kip等一系列问题。

目前看来有三种方法解决这种办法：

（1）因为大气层三件套是atmosphere+hekate+sigpatch，启动系统的方法是四种，fusee大气层自动识别不能再加载KIP补丁，但是通过Hekate的fss0引导的真实（破解）系统，虚拟（破解）系统的KIP是通过bootloader/patch.ini实现，所以不受大气层1.7.0升级导致不能玩破解游戏的影响。

https://www.tekqart.com/thread-289271-1-1.html

左起1，2，3都是fss0引导，最右4是fusee引导。

（2）sigpatch可以是IPS加载，也可以是通过sys-patch的插件签名补丁的方法，目前原版sys-patch被删库，后续有大神接着开发，论坛有转载，相当于不需要sigpatch组件，直接在破解系统里sysmodule启动，通过Tesla选择是否开启sigpatch，这样就能玩破解游戏了。

所以这种三件套（也可以说四件套）=atmosphere+hekate+sys-patch+tesla，Tesla用于调用sys-patch的菜单。

https://www.tekqart.com/thread-382597-1-1.html

（3）大神编译大气层1.7.0的核心文件，atmosphere/package3，atmosphere/stratosphere.romfs，可以把loader patch限制去掉，还可以把sigpatch的fs补丁内置，payload引导fusee.bin是不需要编译的。

https://www.tekqart.com/thread-382514-1-1.html

以上三种方法没区别，用哪种结果都一样，但是第一种作为以前的延续，使用起来相对简单些，也就是AK一直以来发布的可覆盖的大气层三件套文件

https://www.tekqart.com/thread-321617-1-1.html

可以覆盖，只是在Hekate_ipl.ini里不选择fusee引导（cfw auto），也是作为1.7.0大气层之后的解决玩破解游戏的方法。
