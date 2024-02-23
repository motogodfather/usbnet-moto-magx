# usbnet-motomagx-
Solve the problem that Motorola magx models cannot use usbnet on linux 5.0+ kernel.

基于GodFox版本修改，https://github.com/OpenMagx/usbnet

motorola magx手机在不能通过usbnet方式连接linux 5.0及以上的内核的系统

编译代码中的两个驱动并安装能解决这个问题

使用方法：
	1.切换到源代码路径
	2.make
	3.sudo make install
	
ZN5\U9\E8\EM30\VE66\EM35手机在Linux mint 21.3测试成功

连接手机方法：
	1.在手机上的终端执行 ifconfig usbl0 192.168.16.2
	2.连接电脑到手机
	3.尝试使用telnet、samba、webserver、ssh！

 部分系统不能自动加载zaurus模块：
 编辑/etc/modules-load.d/modules.conf
 添加 zaurus
 
