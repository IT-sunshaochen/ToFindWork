<!--
 * @Date: 2022-10-31 19:56:48
 * @LastEditors: sunshaochen 805960031@qq.com
 * @LastEditTime: 2022-10-31 20:20:50
 * @FilePath: \ToFindWork\linux常用命令.md
-->
# 查看ip地址
	ip a
	ip addr
# ping网络(测试网络连通)
	ip 目标机器的ip
# 查看系统时间
	date
# 注销
	logout
# 关机
	shutdown now
# 重启
	reboot
# 清屏
	clear
   

/bin	所有用户可用的基本命令存放的位置	windows没有固定的命令存放目录
/sbin	需要管理员权限才能使用的命令	
/boot	linux系统启动的时候需要加载和使用的文件	
/dev	外设连接linux后，对应的文件存放的位置	类似Windows中的U盘，光盘的符号文件。
/etc	存放系统或者安装的程序的配置文件,注册服务等	类似windows中的注册表，
/home	家目录，linux中每新建一个用户，会自动在home中为该用户分配一个文件夹	类似windows中的"我的文档"，每个用户有自己的目录。
/root	root账户的家目录，仅供root账户使用	类似windows中的Administrator账户的"我的文档"
/lib	linux的命令和系统启动，需要使用一些公共的依赖，放在lib中，类似我们开发的代码执行需要引入的jdk的jar	
/usr	很多系统软件的默认安装路径	类似windows中的C盘下的Program Files目录。
/var	系统和程序运行产生的日志文件和缓存文件放在这里
