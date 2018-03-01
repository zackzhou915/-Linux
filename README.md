## Linux常用命令(来自黑马)

### 文件管理
1) 查看文件信息：ls
2) 输出重定向命令：>
3) 分屏显示：more
4) 管道：|
5) 清屏：clear
6) 切换工作目录：cd
7) 显示当前路径：pwd
8) 创建目录：mkdir
9) 删除目录：rmdir
10) 删除文件：rm
11) 建立链接文件：ln
12) 查看文件内容：cat
13) 拷贝文件：cp
14) 移动文件：mv
15) 获取文件类型：file
16) 归档管理：tar 
17) 文件压缩：gz(-zcvf)、bzip2(-jcvf)、zip -r
18) 文件解压：tar -xvf、unzip -d
19) 查看命令位置：which

### 用户、权限管理
1) 查看当前用户：whoami
2) 退出登录账户：exit
3) 切换用户：su
4) 添加、删除组账户：groupadd、groupdel
5) 修改用户所在组：usermod
6) 添加用户账号：useradd
7) 设置用户密码：passwd
8) 删除用户：userdel
9) 查询用户登录情况：last
10) 修改文件权限：chmod
11) 修改文件所有者：chown
12) 修改文件所属组：chgrp

### 系统管理
1) 查看进程信息：ps
2) 动态显示进程：top
3) 终止进程：kill
4) 后台程序：&、jobs、fg
5) 关机重启：reboot、shutdown、init
6) 查看或配置网卡信息：ifconfig
7) 测试远程主机连通性：ping

### vi常用命令
##### 插入模式
a 光标位置右边插入文字  
i 光标位置当前初插入文字  
o 光标位置下方开启新行  
O 光标位置上方开启新行  
I 光标所在行首插入文字  
A 光标所在行尾插入文字  
##### 退出
:wq 保存退出  
:q! 强制退出  
##### 修改
dd 剪切  
yy 复制  
p 粘贴  
u 撤销  
ctrl+r 恢复  
##### 定位
gg 第一行行首  
G 最后一行行尾  
ctrl+f 前滚动  
ctrl+b 后滚动  
##### 查找
/关键字 查看指定关键字，n下一个，N上一个  

### SSH
1) 远程登录：ssh -l username hostip
2) 文件传输 
本地文件复制到远程 scp FileName RemoteUserName@RemoteHostIp:RemoteFile
本地目录复制到远程 scp -r FolderName RemoteUserName@RemoteHostIp:RemoteFolder
远程文件复制到本地 scp RemoteUserName@RemoteHostIp:RemoteFile FileName
远程目录复制到本地 scp -r RemoteUserName@RemoteHostIp:RemoteFolder FolderName
