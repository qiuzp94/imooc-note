* 文档型: 文件相关命令（touch、cat、echo、rm、vi、cd）
* 硬件型: 磁盘/进程/服务/网络
* 功能型: 压缩/解压，下载，远程

[Linux入门之常用命令用法解析](https://qiuzp.com/2020/04/03/Linux%E5%85%A5%E9%97%A8%E4%B9%8B%E5%B8%B8%E7%94%A8%E5%91%BD%E4%BB%A4%E7%94%A8%E6%B3%95%E8%A7%A3%E6%9E%90/)

## 下载/压缩/解压
* `wget 资源` 下载资源
* `tar zxvf 资源名.tar.gz` 解压资源（z是代表gz后缀压缩文件，x代表解压缩，v代表显示所有解压过程，f代表的是使用归档的名字）
* `tar zcvf 压缩后资源名.tar.gz 压缩前文件` 压缩资源

## grep命令-查看进程
* `ps -ef | grep docker`查看docke进程情况
* `kill -9 pid号` 终止 某个pid号 的进程

## 查看系统服务状态
* `service sshd status` 查看sshd的运行状态
* `service sshd stop` 关闭sshd
* `service sshd restart` 重启sshd

## 选择题
`tar`是压缩与解压命令
`touch`是用来修改文件时间戳，或者新建一个不存在的文件
`cat`查看命令，连接文件或标准输入并打印
`netstat`用于显示各种网络相关信息，如网络连接，路由表，接口状态。

