`cat /etc/hostname` 查看服务器名称
`netstat -anlp | grep sshd`查看ssh服务进程情况

`vi /etc/ssh/sshd_config`修改ssh配置
把ssh的端口 port 22改为不常用的10022 减少被攻击的概率

`yum install -y policycoreutils-python`
`semanage port -a -t ssh_port_t -p tcp 10022`

`semanage port -l | gerp ssh`
`semanage port -d -t ssh_port_t -p tcp 10022`

`semanage port -l | gerp ssh`
`service sshd restart`

用ssh密钥方式连接
`cd ~/.ssh`
`ssh-keygen`

`vi config`
新增内容如下

```
Host 主机名
    Port 端口号
    HostName ip地址
    User root
    IdentitFile ~/.ssh/id_rsa
    IdentiteOnly yes
```
然后测试连接 `ssh 主机名`
`pwd`查看路径


`cd ~/.ssh/`

`mkdir -p ~/.ssh`
`vi authorized_keys`

`cat ~/.ssh/id_rsa.pub`