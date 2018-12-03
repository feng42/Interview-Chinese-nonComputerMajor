
# 1 命名提示符
(#)
# 2 目录操作
1. ls
显示目录内容
ls -a

2. cd
切换目录
cd /usr/bin/python/

3. mkdir
创建目录
mkdir -p /zf/movie/jp/yua_mikami

4. rmdir
删除目录
rmdir aoi

5. tree
树形显示
tree /etc/

# 3 文件操作
1. touch 
“摸”一下文件
touch bols
2. stat
查看访问时间、修改时间、状态修改时间
stat bols
3. cat
查看文件内容
cat bols
4. more
分屏显示
5. less 
分行显示
6. head
显示文件开头
7. tail 
显示文件末尾
tail -f 监听新增内容
8. ln
建立文件软硬链接
ln -s -f /root/yua /tmp/

# 4 目录和文件都可用的
1. rm
删除
rm -f bols
2. cp 
复制
cp /Interview/* /tmp/
3. mv
剪切
mv yua /tmp/
4

# 5 权限管理
0. 
    -      rw-      rw-     r--
文件类型  所有者   所属组   其他人
1. chmod[change file mode bits]
添加权限
chmod [ugoa][[+-=][perms]]
chmod 755 yua
2. chown[change file owner and group]
修改所有者和所有组
chown user yua
3. chgrp[change group onwership]
修改文件和目录所属组
chgrp user test2
4. umask默认权限

# 6 帮助命令
1. man[manual pages]
显示联机使用手册
man ls
2. help
获取shell内置命令帮助
help tree

# 7 搜索
1. whereis
只能搜索系统命令
whereis ls
2. which
还能找到别名
which ls
3. locate
按名搜索
locate install.log
4. find
还可以按照权限、大小、时间、inode搜索
find / -name yum.conf

# 8 压缩与解压缩
1. zip
zip -r dir1.zip dir1 
unzip dir1.zip
2. gzip
gzip -c(保留源文件)
gunzip -r test/
3. bz2
bzip2 anaconda-ks.cfg
bunzip2 anaconda-ks.cfg.bz2
4. tar
tar -cvf ana.tar anaconda-ks.cfg /tmp/
tar -xvf anaconda.tar

# 9 关机和重启
1. sync
内存数据保存到硬盘
sync
2. shutdown
关机
shutdown -r 05:30
3. reboot
4. halt
5. poweroff
6. init
init 0
init 6

# 10 网络命令
1. setup[RedHat专有]
2. ifconfig
查看和临时修改ip
3. ifdown
4. ifup
5. ping
 测试网络中主机通信情况
ping -b 172.17.255.255
6. netstat
输出网络连接、路由表、接口设计、伪装连接和组播成员
7. write
向其他用户发送信息
write user1 pts/1
8. wall
所有登录用户发信息
9. mail
发送电子邮件
mail user1




